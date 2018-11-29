# 1.6 Prikaz i pregledavanje metapodataka pomoću OpenRefine-a

[OpenRefine](http://www.openrefine.org) pruža grafičko sučelje za analizu i transformaciju podataka, slično tabličnim kalkulatorima poput MS Excel ili LibreOffice Calc itd. Ovaj softver koristimo jer se pomoću grafičkog korisničkog sučelja možete dobiti mogućnost brzog pregleda podataka, a uz to program omogućava baratanje s različitim metapodatkovnim formatima. 

## Instalacija OpenRefine-a

Na mrežnom sjedištu [OpenRefinea](http://openrefine.org/download.html) ponuđene su različite verzije pograma [Download]. Za rad na MacOS-u preuzmite zadnju verziju 3.1 u .dmg formatu. 

## Pokretanje OpenRefine-a

Na MacOS-u otvorite `Application -- OpenRefine`

U pregledniku otvorite sljedeću IP adresu: [http://127.0.0.1:3333](http://127.0.0.1:3333)s.

## Vježba: Učitavanje podataka iz poglavlja 1.5 u Openrefine

U izborniku "Create Project" odaberite gumb "Pronađi" i odaberite XML datoteku koju smo pohranili u poglavlju 1.5. Nakon toga odaberite u sljedećem prozoru opciju "parsanja" podataka iz "XML files", a nakon toga u prikazu odarite liniju ```<record xmlns:xs="http://www.w3.org/2001/XMLSchema">``` te nakon toga u gornjem desnom kutu odaberite gumb "Create Project".

OpenRefine "ne razumije" MARC format i stoga interpretira podatke kao bilo koju drugu XML datoteku. Kada datoteku prvi put otvorite u OpenRefinu, prikazat će se brojevi i kodoovi MARC polja koji čine strukturu stabla XML datoteke. 

Značenje MARC brojeva i kodova morate poznavati ili pronaći njihovu značenje u nekom od brojnih dostupnih web izvora. 

## Vježba: Obradite pregled podataka (strukture) pomoću faceta i filtera 

* Pogledajte kratki uvod u OpenRefine na [YouTubeu](https://www.youtube.com/watch?v=B70J_H_zAWM)
* Konzultirajte OpenRefine dokumentaciju u kojoj se posebno bave [problematikom facetiranja](https://github.com/OpenRefine/OpenRefine/wiki/Faceting) i isprobajte različite facete.
* Dobra vježba dostupna je na Library Carpentry OpenRefine: [Basic OpenRefine Functions I: Working with columns, sorting, faceting, filtering and clustering](https://data-lessons.github.io/library-openrefine/03-basic-functions-I/)

## Zatvaranje OpenRefine sesije


