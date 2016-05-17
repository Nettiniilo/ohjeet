# Nettiniilon ohjelmistopäivitys ja resetointi

<!-- toc -->

Nettiniilon ohjelmistoa (firmware) on mahdollista päivittää valmistajan jakelemilla päivitystiedostoilla. Päivitykset tuovat uusia ominaisuuksia ja/tai korjaavat havaittuja puutteita.

## Nettiniilon ohjelmiston päivittäminen

Nettiniilon ohjelmistopäivitys on teknisesti mahdollista tehdä sekä {{ book.netti.nicename | lower }}ssa että {{ book.abitti.nicename }}ssa; on kuitenkin suositeltavaa tehdä päivitys {{ book.netti.nicename | lower }}ssa koska mikäli päivitys tehdään {{ book.abitti.nicename }}ssa, ei päivityksen valmistumisesta tule käyttäjälle ilmoitusta.

Suorita ohjelmistopäivitys seuraavasti:

1. Lataa Nettiniilon zip-muotoinen päivitystiedosto sähköpostitse valmistajalta saamastasi latauslinkistä.
2. Pura päivitystiedoston sisältö jonkun muistitikun juurikansioon.
	- Muistitikulle ilmestyvät tällöin tiedostot <kbd>nettiniilo.bin</kbd> ja <kbd>nettiniilo.bin.md5</kbd>.
3. Käynnistä Nettiniilo ja odota, että laitteen WLAN-valo syttyy.
4. Varmista, että Nettiniilo on {{ book.netti.nicename | lower }}ssa:
	- WPS-valon ei siis kuulu palaa.
	- Mikäli WPS-valo palaa, paina ko. nappia kevyesti ja odota.
	- WPS-nappi alkaa parin sekunnin viiveellä vilkkua ja vilkkuu parikymmentä sekuntia.
	- Kun WPS-valo lopettaa vilkkumasta ja jää pois päältä, on laite {{ book.netti.nicename | lower }}ssa.
5. Liitä tavallisesti (eli ei Abittiin) käynnistetty (Windows/Apple/Linux) tietokone ethernet-kaapelilla Nettiniilon *PoE LAN* -porttiin.
6. Avaa Internet-selain em. tietokoneella ja kirjaudu Nettiniilon hallintapaneeliin osoitteessa <{{ book.netti.urls.admin }}>
	- Mikäli et pääse hallintapaneeliin kokeile näitä:
	- Irrota ethernet-kaapeli jommasta kummasta päästä noin 10 sekunniksi; kiinnitä kaapeli takaisin.
	- Katkaise mahdollinen langattoman verkon yhteys.
	- Varmista ettei selaimessasi ole välityspalvelin käytössä ja jos on, poista se tilapäisesti käytöstä.
	- Kokeile uudelleen päästä hallintapaneeliin <{{ book.netti.urls.admin }}> .
7. Mene hallintapaneelissa *Ohjelmistopäivitys*-näkymään.
8. Kiinnitä vaiheen 2 mukainen muistitikku Nettiniilon USB-porttiin ja odota pari sekuntia.
9. Paina kohdan 7 mukaisessa näkymässä *Päivitä ohjelmisto* -nappia.
10. Odota noin kolme (3) minuuttia, älä klikkaile muuta.
	- ***ÄLÄ IRROTA NETTINIILON VIRTAJOHTOA KESKEN OHJELMISTOPÄIVITYKSEN!!***
	- Noin päivityksen puolivälissä Nettiniilon valot sammuvat virtavaloa (PWR) lukuunottamatta ja alkavat sitten syttyä uudelleen.
	- Saat selainikkunaasi ilmoituksen kun päivitys on valmis.


## Nettiniilon resetointi eli palauttaminen tehdasasetuksiin

Nettiniilo on mahdollista palauttaa viimeisimmän ohjelmistopäivityksen mukaisiin oletusasetuksiin. Tehdasasetusten palauttaminen asettaa kaikki salasanat ja muut asetukset oletusarvoihinsa.

Resetointi tapahtuu seuraavasti:

1. Käynnistä Nettiniilo ja odota, että WLAN-valo syttyy.
	- Resetointia varten Nettiniilo voi joko {{ book.netti.nicename | lower }}ssa tai {{ book.abitti.nicename }}ssa.
3. Pidä Nettiniilon pohjassa oleva `Reset`-näppäin pohjassa noin 8 sekunnin ajan.
4. Nettiniilo käynnistyy nyt uudestaan ja kaikki asetukset palautuvat viimeisimmän ohjelmistopäivityksen mukaisiin oletusarvoihin.