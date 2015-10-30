# Ongelmatilanteita ja ratkaisuehdotuksia

## Yleiset

Nämä ohjeet ovat joko yleisiä tai koskevat sekä Abitti- että *{{ book.netti.nicename }}*a.

| # | Ongelman kuvaus | Ratkaisuehdotus |
|---|-----------------|-----------------|
| 1 | Vaihdoit Nettiniilon moodia (*{{ book.abitti.nicename }}*sta *{{ book.netti.nicename }}*in tai päinvastoin) ja olit vaihtohetkellä liittyneenä Nettiniiloon joko ethernet-kaapelilla tai langattomasti. Moodin vaihdon jälkeen et saa yhteyttä esimerkiksi Nettiniilon hallintapaneeliin. | **a)** Irroita koneen ja Nettiniilon välinen ethernet-kaapeli noin 10 sekunniksi ja liitä se sitten takaisin ja kokeile uudestaan.<br>**b)** Jos käytit langatonta yhteyttä, katkaise se ja yhdistä uudestaan. |
| 2 | Pääset Nettiniilon tiedostojenjakoon (*{{ book.abitti.nicename }}*ssa: <{{ book.abitti.urls.share }}>, *{{ book.netti.nicename }}*ssa: <{{ book.netti.urls.share }}>), mutta et saa osaa tiedostoista ladattua vaikka tiedosto näkyy tiedostolistauksessa. | Onko ongelmia aiheuttavien tiedostojen tiedostonimissä ääkkösiä tai lainausmerkkejä? Mikäli kyllä, kyseiset merkit on poistettava tiedostonimestä, jotta tiedosto on käytettävissä Nettiniilon materiaalinjaon kautta. |


## *{{ book.abitti.nicename }}*

*{{ book.abitti.nicename }}* on tarkoitettu käytettäväksi YTL:n Abitti-nimisen sähköisen kurssikoejärjstelmän kanssa. Mikäli et löydä kysymykseesi vastausta tästä listasta tai sisällysluettelon *{{ book.abitti.nicename }}*n alla olevista ohjeista, ota yhteyttä.

| # | Ongelman kuvaus | Ratkaisuehdotus |
|---|-----------------|-----------------|
| 1 | Et pääse Abitti-palvelimelta Nettiniilon hallintapaneeliin osoitteeseen <http://10.10.0.10:8020> | Abitti-järjestelmän v37 päivityksen myötä (17.8.2015 alkaen) Nettiniilon hallintapaneeliin mennään osoitteessa <{{ book.abitti.urls.admin }}>. Huomaa, että Nettiniilon ohjelmistoversion on oltava v1.0.0 tai uudempi, jotta hallintapaneeliin pääsee *{{ book.abitti.nicename }}*ssa Abitti-palvelimen v37 tai uudemmilla versioilla. Jos olette päivittäneet Abitti-tikut v37 tai uudempiin, mutta ette ole päivittäneet Nettiniiloa, ei Nettiniilon ohjelmistoa voi päivittää *{{ book.abitti.nicename }}*ssa vaan päivitys on tehtävä *{{ book.netti.nicename }}*n kautta. |
| 2 | Videot ja äänet eivät toimi opiskelijan koneelta Nettiniilon tiedostonjakoa osoitteessa <{{ book.abitti.urls.share }}> käytettäessä. | Varmista, että käytössänne on Abitti-opiskelijantikkujen versio 45 (25.9.2015) tai uudempi. Abitti-järjestelmän versioista v37 (17.8.2015), v40 (4.9.2015) ja v43 (noin 15.9.2015 paikkeilla) puuttuu mediatoisto-ohjelma, jota videoiden ja äänien katseluun/kuunteluun tarvitaan. |
| 3 | Opiskelijat putoilevat satunnaisesti Nettiniilon tarjoamasta verkosta. | **a)** Oletuksena Nettiniilo valitsee käynnistyessään käyttöönsä mahdollisimman vähän liikennöidyn kanavan; Nettiniilon käynnistäminen uudelleen saattaa siis auttaa.<br>**b)** Voit kysyä atk-vastaavaanne tarkistamaan esimerkiksi Android-puhelimille ilmaiseksi tarjolla olevalla [Wifi Analyzer](https://play.google.com/store/apps/details?id=com.farproc.wifi.analyzer&hl=fi) -ohjelmalla onko Nettiniilon kyseisellä hetkellä käyttämä liikennöintitaajuus päällekkäin ja signaalitasoltaan heikompi kuin joku muu samalla taajuudella ("kanavalla") liikennöivä langaton verkko. |


## *{{ book.netti.nicename }}*

Mikäli et löydä kysymykseesi vastausta tästä listasta, yllä olevasta *Yleiset*-kohdasta tai sisällysluettelon *{{ book.netti.nicename }}*n alla olevista ohjeista, ota yhteyttä.

| # | Ongelman kuvaus | Ratkaisuehdotus |
|---|-----------------|-----------------|
| 1 | Et pääse liittymään Nettiniilon tarjoamaan langattomaan verkkoon. | **a)** Varmista, että oikea verkko on valittuna ja salasana on varmasti kirjoitettu oikein.<br>**b)** Mikäli WLAN-verkon salasanaa on hiljattain vaihdettu Nettiniilon hallintapaneelista, mutta verkon nimeä ei, saatat joutua asettaman kyseisen verkon "unohdetuksi" käyttöjärjestelmässään eli poistamaan mahdollisen automaattisen liittymisyrityksen ko. verkkoon ja liittymään sitten uudestaan. |
| 2 | Et saa opettajan koneella yhteyttä Nettiniilon hallintapaneeliin. | **a)** Varmista, että sinulla on yhteys ethernet-kaapelilla tietokoneestasi Nettiniilon PoE LAN -porttiin ja että Nettiniilo on *{{ book.netti.nicename }}*ssa eli WPS-valo on sammuksissa.<br>**b)** Varmista ettet ole samaan aikaan liittyneenä Nettiniiloon myös langattomasti. Mikäli sinulla on yhtä aikaa yhteys Nettiniiloon sekä Ethernet-johdolla että langattomasti, saattaa koneesi "hämmentyä".<br>**c)** Mikäli et saa yhteyttä hallintapaneeliin kun vain ethernet-yhteys on käytössä, kokeile irroittaa ethernet-kaapeli ja liittyä Nettiniiloon langattomasti. |
| 3 | Pääset liittymään Nettiniilon tarjoamaan langattomaan verkkoon, mutta et pääse rekisteröitymään (syöttämään nimeäsi). | **a)** Varmista, että selaimessa ei ole välityspalvelin käytössä.<br>**b)** Mene rekisteröitymistä varten nettiselaimella osoitteeseen <{{ book.netti.urls.landing }}><br>**c)** Applen kannettavilla laitteilla älä käytä Safari-selainta vaan Chromea. |
| 4 | Pääset liittymään Nettiniilon tarjoamaan langattomaan verkkoon ja olet rekisteröitynyt Nettiniiloon eli syöttänyt nimesi, mutta et silti pääse nettiin. | **a)** Onko Nettiniilon WAN/LAN-portista kytketty ethernet-kaapeli koulun seinään?<br>**b)** Tai vaihtoehtoisesti onko yhteys nettiin muodostettu mokkulan kautta?<br>**c)** Yritätkö mennä https-osoitteeseen, mutta kyseinen osoite ei ole osoiterajauksen sallittujen osoitteiden joukossa? Mikäli kyllä, Nettiniilo ei teknisestä syystä voi näyttää kustomoitua virheilmoitusta kuten estetyille http-yhteyksille. |
| 5 | USB-muistitikku on liitetty Nettiniiloon, mutta tikun sisältö ei näy *{{ book.netti.nicename }}*n materiaalinjako-osoitteessa <{{ book.netti.urls.share }}> | Toimiiko tikku tietokoneeseen kytkettäessä normaalisti? Mikäli ei, varmista ensin toimivuus tietokoneeseen kytkettäessä. Mikäli kyllä, varmista, että tikun tiedostojärjestelmänä on FAT32; jos et tiedä mitä tämä tarkoittaa, kysy atk-tueltanne. Jos ongelma ei ratkennut, ota yhteyttä laitteen kehittäjään. |
| 6 | Saat Nettiniilon tiedostonjaosta haluamasi tiedoston ladattua, mutta tiedoston avaaminen ei onnistu. | Onko koneellasi asennettuna tarvittava ohjelma kyseisen tiedostotyypin käyttämiseksi? Mikäli ei, asenna tarvittava ohjelma. Vaihtoehtoisesti pyydä tiedoston jakelijaa (opettajaa) jakamaan tiedoston jossain vaihtoehtoisessa, mahdollisesti yleisemmin käytetyssä tiedostomuodossa. |
