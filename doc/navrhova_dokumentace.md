# Návrhová Dokumentace

## Použité jazky:
- html
- css
- javascript    

## Použité programy:
- Visual Paradigm -> UML diagram -> Zkušební verze
- Visual Studio Code -> Práce na samotném kódu -> MIT licence
- Inkscape -> Kreslení jednotlivých kusů oblečení -> GNU licence

## Použité knihovny:
- [Fontawesome](https://fontawesome.com)  

## Poskytovatel údajů o počasí:
- [Openweather](https://openweathermap.org) -> použita free verze  

## Tutoriály  
- [w3schools.com](https://www.w3schools.com) -> CSS + html tutoriály  
- [StackOverFlow.com](https://stackoverflow.com) -> Změna obrázku  
- [ApiCall](https://bithacker.dev/fetch-weather-openweathermap-api-javascript)    

## Popis funkcí
- getLocation() -> kód ve spolupráci s funkcí showPosition() žádá uživatele o povolení zjištění jeho lokace
- showPosition() -> pomocí spolupráce s getLocation() ukládá zeměpisné souřadnice do proměnných, které jsou následně předávány api, spouští funkci apiCall()
- apiCall() -> pracuje s api pomocí funkce fetch() a také volá funkci ulozData(), kterému také data z odpovědi od Api ukládá
- ulozData() -> tato funkce přijímá data z api callu a ukládá je do id, které je následně vypisováno v html kódu, následně díky zjištění teploty určuje také, který model oblečení by měl uživatel dostat  
- pohlavi() -> vytváří proměnnou pohlavi a ukládá ji na "muz"
- Tlacitko() -> funkce, která mění pozadí a upravuje celý desing stránky a pracuje s uživatelem, zda je vlastně žena nebo muž. mění proměnnou vytvořenou funkcní pohlavi()  
- lokaceManualne() - > Umožňuje uživateli zadání vlastní lokace do příslušeného formu, kterou uloží do proměnné.
- enterNaOdeslani() -> Umožňuje uživateli použít klávesu "enter" k odeslání formuláře s lokací.

## CSS
- body, ul -> odstraní okraje
- header -> nastavuje vzhled, umístění a zarovnání headeru
- tlacitko -> nastavuje vzhled, umístění, velikost,.. tlačítka
- datum -> upravuje vzhled textu, který zkazuje aktuální datum
- info -> upravuje vzled třídy s názvem info  
- form-inline -> zajišťuje, aby formulář se neodděloval od tlačítka
- input[type="text] -> upravuje vzhled pole do kterého uživatel zadáva svou požadovanou polohu
- button[id="odeslat"] -> upravuje vzhed tlačítka kterým uživatel odesílá serveru svou požadovanou polohu
- button[id="odeslat"]:active -> mění barvu tlačítka při stisknutí
- textarea:focus, input:focus, button[id="odeslat"]:focus -> odstraňuje outline když uživatel klikne na objekt
- obrazek -> upravuje velikost a parametry obrázků
