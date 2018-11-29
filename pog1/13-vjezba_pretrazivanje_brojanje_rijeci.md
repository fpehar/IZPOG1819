# 1.3 Vježba: Pretraživanje teksta i pobrojavanje riječi pomoću naredbodavnog retka

Naredbodavni redak je neizostavan način rada na ovom i mnogim drugim predmetima na OIZ. Mnoge programe nije moguće pokrenuti \(instalirati)\ ili konfigurirati bez upotrebe naredbodavnog retka. Osim toga rada u naredbodavnom retku omogućuje brži i učinkovitiji rada. 

## Pokretanje naredbodavnog retka \(terminal\)

Zadani program za rad u naredbodavnom retku se na Linux i OSX računalima naziva [terminal](https://help.ubuntu.com/community/UsingTheTerminal). 


## Instalacija programa cURL 

Za sljedeću vježbu potreban nam je program cURL. U većini Linux distribucija je već predinstaliran. To možete projveriti pomoću sljedeće naredbe u terminalu: 

`curl --version`

U slučaju da nije instaliran, u Linux terminalu upišite sljedeću naredbu: 

`sudo apt-get install curl`

Provjerite opet verziju instaliranog curl programa pomoću sljedeće naredbe: `curl --version`

Procedura instalacije se razlikuje na MacOS-u. Postupak je detaljno opisan na [ovoj stranici](https://help.ubidots.com/how-to-with-ubidots/learn-how-to-install-run-curl-on-windowsmacosxlinux), a mi ga bez deteljnih pojašnjenja niže navodimo: 

1. Otvorite terminal
2. Unesite niže navedenu naredbu: 

`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" < /dev/null 2> /dev/null`

3. Sustav će vas tražiti unos admin zaporke koju će vam nastavnik upisati u terminal. 
4. Pokrenite sljedeću naredbu za dovršetak instalacije cURL

`brew install curl`

Provjerite instaliranu verziju programa pomoću naredbe: `curl --version`. Očekujte odgovor sličan ovom: 

`curl 7.54.0 (x86_64-apple-darwin18.0) libcurl/7.54.0 LibreSSL/2.6.4 zlib/1.2.11 nghttp2/1.24.1
Protocols: dict file ftp ftps gopher http https imap imaps ldap ldaps pop3 pop3s rtsp smb smbs smtp smtps telnet tftp
Features: AsynchDNS IPv6 Largefile GSS-API Kerberos SPNEGO NTLM NTLM_WB SSL libz HTTP2 UnixSockets HTTPS-proxy`


## Vježba: Pretraživanje teksta i pobrojavanje riječi

Pokrenite terminal i unesite sljedeće naredbe: 

### Korak 0: Pozicionirajte se u određeni direktorij

Koristite naredbu `cd` za promjenu direktorija i `mkdir` za izradu novog direktorija pod nazivom `WarAndPeace`. 

* `cd Desktop/`
* `mkdir WarAndPeace`
* `cd WarAndPeace`

### Korak 1: Preuzmite "War and Peace" od Lava Tolstoya

* `curl http://www.gutenberg.org/files/2600/2600-0.txt > war_and_peace.txt`
* `cat war_and_peace.txt | less`

Dodatak `>` u prvom retk sprema preuzetu datoteku `2600-0.txt` pod nazivom `war_and_peace.txt`.

Dodatak `| less` prikazuje tekst na način da se krećete s kursorskim tipkama gore/dolje ili pomoću tipke `Enter`. Iz `less` pogleda izlazite pomoću tipke `q`.

### Korak 2: Brojanje redaka, znakova i riječi pomoću naredbe wc

* `wc war_and_peace.txt`

Tri dobivena broja odnose na redak, riječ i znak \(točno tim redosliejdom)\.

### Korak 3: Traženje pojavnosti riječi "war" i "peace"

* `cat war_and_peace.txt | grep -i -ow war | wc`
* `cat war_and_peace.txt | grep -i -ow peace | wc`

Koja riječ se češće pojavljuje u tekstu? Rat ili mir? 

## Pomoć za rad u naredbodavnom retku

* Datoteke i direktoriji: vidi [Cheatsheet](http://cheatsheetworld.com/programming/unix-linux-cheat-sheet/)
* Prekid rada: _**CTRL**_ i _**C**_ ili _**CTRL**_ i _**D**_
* Pomoć za određeni program: _**Program**_** --help**
* Priručnik za korištenje programa: **man **_** Program**_
* Automatsko "odgonetanje" naziva naredbe/datoteke: _**Tab**_
* Povijest korištenja naredbi: _**Kursorska tipka prema gore tj. dolje**_
* Pretraživanje povijesti korištenja naredbi: _**CTRL**_ i _**R**_

Najlakše je odgovore na razne probleme pronaći na webu. Dovoljno je u tražilicu upisati linux + command i dobit ćete more izvora koji će vas uputiti u ispravan korak. 


## Literatura
