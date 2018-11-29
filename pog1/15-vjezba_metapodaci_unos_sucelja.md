# 1.5 Vježba: Učitavanje metapodata pomoću SRU sučelja

Kratica [SRU](http://www.loc.gov/standards/sru/) \(Search/Retrieve via URL\) odnosi se na XML-u utemeljeni protokol za postavljanje upita koristeći CQL \(Contextual Query Language\) kao standardnu sintaksu za predstavljanje upita. 

U sljedećoj vježbi koristit ćemo SRU sučelje [švicarske digitalne knjižnice](http://sru.swissbib.ch).


## Zadatak 1: Učitati 10 zapisa putem SRU sučelja

* Upitni pojam: `open`
* Format:`MARC XML - swissbib`

## Zadatak 2: Učitati podatke u različitim formatima \(npr. Dublin Core\) i usporediti


## Zadatak 3: Pohraniti podatke pomoću curl

primjer marcxml:

```
curl "http://sru.swissbib.ch/sru/search/defaultdb?query=+dc.possessingInstitution+%3D+E27&operation=searchRetrieve&recordSchema=info%3Asrw%2Fschema%2F1%2Fmarcxml-v1.1-light&maximumRecords=10&startRecord=0&recordPacking=XML&availableDBs=defaultdb&sortKeys=Submit+query"  > open-10-marc.xml
```

primjer dc:

```
curl "http://sru.swissbib.ch/sru/search/defaultdb?query=+dc.anywhere+%3D+open+AND+dc.possessingInstitution+%3D+E27&operation=searchRetrieve&recordSchema=info%3Asru%2Fschema%2F1%2Fdc-v1.1-light&maximumRecords=10&startRecord=0&recordPacking=XML&availableDBs=defaultdb&sortKeys=Submit+query" > open-10-dc.xml
```



