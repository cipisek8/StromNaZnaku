# Overview
Kód je rozdělený na 4 hlavní části:
- Seznam (GUIList)
- Prohlížeč lidí (GUIPerson)
- Hledač lidí (Finder)

A ta ==***nejdůležitější***== třída ze všech, ze které dědí obě GUI třídy, bez ní by se to celý program rozpadnul:
- GUICommon

Obě GUI třídy řeší pohyb a visualizaci dat v sobě, třída Main přepíná mezi nima a dává jim společná data a třída Finder dává metody k vyhledávání lidí.

Seznam se ukládá do formátu .png .

---

# Metody
### Finder.FindBoss
Najde nejbližšího šéfa vyhledávaného zaměstnance pomocí ID zaměstnance.
### Finder.FindSalesman
Najde zaměstnance pomocí jeho ID.
### Finder.SetHighestPerson
Nastaví šefa celého stromu.
### Finder.FindNetworkSales
Sečte příjmy šáfa, jeho podzaměstnanců, jejich podzaměstnanců atd.

---

### GUIList.ChangeList / GUIPerson.ChangePerson
Změní list u seznamu nebo změní osobu u prohlížeče.
### GUIList.CreateTemplate / GUIPerson.CreateTemplate
Udělaté šablonu pro neměnící se prvky.
### GUIList.WritePeople / GUIPerson.WritePeople
Napíše data a interaktivní prvky do šablony.
### GUIList.Move / GUIPerson.Move
Detekování tláčítek, kontrola co se má stát.
### GUIList.Select / GUIPerson.Select
Barvení prvků podle toho, kde je cursor.
### GUIList.UpdatePeople
AKtualizace viditelného seznamu lidí.

---

### GUICommon.Line
Vykreslí čáru pod menu tlačítkama.