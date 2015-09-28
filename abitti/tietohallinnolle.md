# Nettiniilo Abitti-moodissa: tietohallinnolle

Näiden ohjeiden tavoitteena on selittää TVT-vastaavien ja tietohallinnon näkökulmasta Nettiniilon käyttämiseen liittyviä yksityiskohtia Nettiniilon Abitti-moodia yhdessa Ylioppilastutkintolautakunnan Abitti-järjestelmän kanssa käytettäessä.


## Abitti-moodissa Nettiniilo toimii kytkimenä

Olleessaan Abitti-moodissa Nettiniilo toimii ethernet-verkon näkökulmasta kytkimenä (Netti-moodissa reitittimenä). Toisin sanoen, Nettiniilo ei Abitti-moodissa ollessaan toimi DHCP-palvelimena eikä siis jaa IP-osoitteita siihen langattomasti tai ethernet-kaapelilla liitetyille laitteille. Päinvastoin Nettiniilo olettaa Abitti-moodissa, että samassa verkossa on joku DHCP-palvelimen roolia toimittava laite. Abitti-koetilapalvelin on YTL:n toimesta ohjelmoitu toimimaan DHCP-palvelimena.



## Nettiniilon firmwaren päivittäminen



## Nettiniilon palauttaminen tehdasasetuksiin

Nettiniilo on mahdollista palauttaa viimeisimmän ohjelmistopäivityksen mukaiseen tehdasasetustilaan. Tehdasasetusten palauttaminen asettaa kaikki salasanat ja muut asetukset oletusarvoihinsa.

Tehdasasetusten palauttaminen tapahtuu seuraavasti:

1. Käynnistä Nettiniilo ja odota, että WLAN-valo syttyy.
2. Pidä Nettiniilon pohjassa oleva `Reset`-näppäin pohjassa noin 8 sekunnin ajan.
3. Nettiniilo käynnistyy nyt uudestaan ja tehdasasetukset ovat palautuneet.

## Mahdollisuus hybridiverkkoon

Oletusarvoisesti Nettiniiloa käytettäessä kaikki opiskelijat liittyvät Nettiniilon muodostamaan verkkoon ja sitä kautta Abitti-koetilapalvelimeen langattomasti. Nettiniilon avulla on kuitenkin mahdollista muodostaa myös hybridiverkko, jossa osa opiskelijoista liittyy verkkoon langattomasti ja osa ethernet-kaapelien kautta.

### Syitä hybridiverkon muodostamiseen

Hybridiverkon muodostaminen on varteenotettava vaihtoehto esimerkiksi seuraavissa tilanteissa:

- osassa päätelaitteista langaton verkko ei syystä tai toisesta toimi Abitti-opiskelijantikun käyttöjärjestelmää käytettäessä
- halutaan liittää enemmän päätelaitteita samaan verkkoon kuin Nettiniilo jaksaa langattomasti palvella (Nettiniilon pitäisi pystyä palvelemaan Abitti-moodissa jopa 50-60 opiskelijaa)

### Hybridiverkon muodostaminen

Muodostaaksesi hybridiverkon tarvitset Nettiniilon ja Abitti-palvelimen lisäksi kytkimen (switch) sekä luonnollisesti tarvittavan määrän ethernet-kaapeleita.

Toimi seuraavasti verkon muodostamiseksi:

1. Käynnistä Nettiniilo kytkemällä siihen virta
	- odota että WLAN-valo syttyy
	- varmista, että laite on Abitti-moodissa eli että WPS-valo palaa
2. Käynnistä Abitti-koetilapalvelin.
3. Liitä Nettiniilo PoE LAN -portistaan ethernet-johdolla kytkimeen.
4. Liitä Abitti-palvelin ethernet-johdolla kytkimeen (ei siis Nettiniiloon).
5. Liitä ethernet-kaapelilla verkkoon liitettävät opiskelijoiden koneet kytkimessä vielä vapaana oleviin portteihin.



## WLAN-verkon käyttämän taajuuden/kanavan käsivalinta

Oletusarvoisesti Nettiniilon langaton verkko valitsee laitteen käynnistyksen yhteydessä käyttämäkseen liikennöintitaajuudeksi käynnistymishetkellä ko. tilassa mahdollisimman vähän käytetyn 2.4 GHz liikennöintialueella olevan WLAN-taajuuden/-kanavan.

On kuitenkin tilanteita, joissa on perusteltua asettaa Nettiniilo käyttämään aina samaa taajuutta/kanavaa. Näin esimerkiksi jos Nettiniilot asennetaan opetusluokkiin kiinteästi ja halutaan vierekkäisissä tiloissa olevat Nettiniilot käyttämään keskenään eri taajuuksia.

Taajuuden/kanavan käsivalinta ei ole tällä hetkellä mahdollista, mutta on tulossa mahdolliseksi ohjelmistopäivityksen myötä myöhemmin.



## Suorituskapasiteetti

Nettiniiloa on testattu valmistajan puolesta Abitti-moodissa enimmillään 60 yhtäaikaisesti Nettiniilon langattomaan verkkoon liittyneellä kannettavalla tietokoneella. Testaus suoritettiin Vaskivuoren lukiolla Vantaalla 25.4.2015.

- Abitti-palvelimena toimi tavallinen pöytäkone
- 60 Abitti-opiskelijantikuilta käynnistettyä langattomasti liittynyttä konetta
- Ylioppilastutkintolautakunnan kevyt ja raskas kuormitustesti ok
- 250 kbit/s videon katsominen Nettiniilon materiaalinjaon kautta oppilaskoneille streamattuna
	- videon katselu aloitettiin pienellä porrastuksella
	- porrastus johtui siitä, että koneet piti "juosta läpi" play-nappia klikaten