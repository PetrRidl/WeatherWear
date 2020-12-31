# Návrhová Dokumentace
## Použité jazky:
- html
- css
- javascript

## Popis funkcí
- getLocation() -> kód ve spolupráci s funkcí showPosition() žádá uživatele o povolení zjištění jeho lokace
- showPosition() -> pomocí spolupráce s getLocation() ukládá zeměpisné souřadnice do proměnných, které jsou následně předávány api, spouští funkci apiCall()
- apiCall() -> pracuje s api pomocí funkce fetch() a také volá funkci ulozData(), kterému také data z odpovědi od Api ukládá
- ulozData() -> tato funkce přijímá data z api callu a ukládá je do id, které je následně vypisováno v html kódu, následně díky zjištění teploty určuje také, který model oblečení by měl uživatel dostat  
- pohlavi() -> vytváří proměnnou pohlavi a ukládá ji na "muz"
- Tlacitko() -> funkce, která mění pozadí a upravuje celý desing stránky a pracuje s uživatelem, zda je vlastně žena nebo muž. mění proměnnou vytvořenou funkcní pohlavi()

## CSS
- body, ul -> odstraní okraje
- header -> nastavuje vzhled, umístění a zarovnání headeru
- tlacitko -> nastavuje vzhled, umístění, velikost,.. tlačítka
- datum -> upravuje vzhled textu, který zkazuje aktuální datum
- info -> upravuje vzled divu s názvem info
