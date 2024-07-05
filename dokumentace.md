# Overview
Kód je rozdělený na 4 hlavní části:
- Seznam (GUIList)
- Prohlížeč lidí (GUIPerson)
- Hledač lidí (Finder)

A ta ==***nejdůležitější***== třída ze všech, ze které dědí obě GUI třídy, bez ní by se to celý program rozpadnul:
- GUICommon

Obě GUI třídy řeší pohyb a visualizaci dat v sobě, třída Main přepíná mezi nima a dává jim společná data a třída Finder dává metody k vyhledávání lidí.

---

# Metody
## Finder
### FindBoss
Najde nejbližšího šéfa vyhledávaného zaměstnance pomocí ID zaměstnance.
### FindSalesman
Najde zaměstnance pomocí jeho ID.
### SetHighestPerson
Nastaví šefa celého stromu.
### FindNetworkSales
Sečte příjmy šáfa, jeho podzaměstnanců, jejich podzaměstnanců atd.

---

## GUIList / GUIPerson
### ChangeList / ChangePerson
Změní list u seznamu nebo změní osobu u prohlížeče.
### CreateTemplate
Udělaté šablonu pro neměnící se prvky
### WritePeople
Napíše data a interaktivní prvky do šablony.
### Move
Detekování tláčítek, kontrola co se má stát.
### Select
Barvení prvků podle toho, kde je cursor.
### UpdatePeople (jen u GUIList)
AKtualizace viditelného seznamu lidí.

## GUICommon
### Line
Vykreslí čáru pod menu tlačítkama.