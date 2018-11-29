# 1.4 Metapodatkovni standardi i sučelja

## Pitanja

* Koji podatkovni formati su u knjižničarstvu uobičajeni? 
* Preko kojih sučelja je moguće pristupiti podacima? 

## Uvod 


## Metapodatkovni formati i standardi

Prisjetite se svega što ste čuli na prethodno odslušanim i položenim predmetima. 

Postoje različite definicije metapodataka, ovisno o perspektivi ili kontekstu \(npr. knjižinčari, arhivisti, ITvci i dr.\). U načelu su to **strukturirani "podaci o podacima"**, dakle formalni opisi mnoštva stvari \(tekst, slika, objekt, osoba i ostalo\). Uloga metapodataka je, između ostalog, olakšati pronalazak, indentifikaciju, odabir i pristup određenom izvoru. Metapodaci se mogu pohraniti unutar objekta ili u datoteci koja je odvojena od opisanog objekta. Slikovni podaci poput JPG sadržaje ugrađene metapodatke \(datum snimanja, razlučivost i dr.\).

S obzirom da su zahtjevi za metapodacima osjetljivi na kontekst, razvili su se razni standardi. Primjeri u knjižničarstvu su **PICA, MODS, DC, MAB, MARC21, METS, EAD, TEI, LIDO **. Ti se standardi mogu \(tehnički\) prevesti u različite formate \(tekst, XML\). Pravila standarda često se dokumentiraju u tzv. **Shemama**, koji se mogu koristiti za provjeru (tehničke) usklađenosti sa standardima. Ako se primjena želi preciznije odrediti, pa čak kombinirati elemente iz različitih standarda, to se navodi i opisuje u tzv. **aplikacijskom profilu**.

Za spajanje metapodatke iz različitih izvora potrebno je "prevesti" podatke iz različitih izvornih shema \(MARC21, PICA\) u uniformnu \(ujednačenu\) ciljnu shemu. Ovaj se proces naziva **mapiranje** \(engl. **mapping** ili "Crosswalk"\). Pritom se, ovisno o shemi, gubi više ili manje informacija. Postoje **crosswalk** standardni između različitih metapodatkovnih standarda. Međutim, moramo biti svjesni činjenice da mnoge ustanove u stvarnosti koriste samo neka metapodatkovna polja. Stoga bi uvijek trebalo pregledati podatke i utvrditi koja se polja stvarno koriste. Zbog navedenog razloga se većina mapiranja provodi na temelju standardnih "poprečnih šetnji" i djelomično na temelju podataka iz analiziranog uzorka. 

## Sučelja

Za razmjenu metapodataka koriste se sučelja poput **Z39.50, SRU ili OAI-PMH**. Pružatelji usluga na temelju internog formata podataka izrađuju preostale "izlazne formate" \(engl. **export formats**\). U tu svrhu potrebno je odrediti podudarna polja i to se naziva "mapiranje" ili ["poprečna šetnja"](https://en.wikipedia.org/wiki/Schema_crosswalk). Ako se svi podaci iz izvornog formata ne uklapaju u ciljni \(najniži zajednički nazivnik, npr. metapodatkovni format **Dublin Core**\) tada moramo računati da ćemo određeni informacije izgubiti tijekom provedbe postupka. Preuzimanje podataka putem posebno razvijenih sučelja naziva se **Harvesting** \(ili pobiranje\). 

## Agregatori

Mnoge neprofitne organizacije prikupljaju podatke iz različitih izvora kako bi ih grupirale i stavile na raspolaganje u jedinstvenoj shemi. Ovaj se proces često naziva agregacija, pružatelji podataka su nazivaju agregatori. Primjeri:

* Mreže knjižnica \(ili skupne knjižnice\)
* CrossRef: članci iz digitalnih časopisa s DOI oznakom
* Akademske tražilice i repozitoriji \(uglavnom u otvorenom pristupu\)
* Nacionalne digitalne knjižnice ili Europeana

## Interoperabilnost metapodataka

* dogovor oko jednog sveobuhvatnog metapodatkovnog formata nije realan \(opisi različitih izvora, različiti zahtjevi, različite tradicije opisa ...\)
* Interoperabilnost između formata mora se postići pomoću alata
* zahtjeva otvorene standarde

## Literatura