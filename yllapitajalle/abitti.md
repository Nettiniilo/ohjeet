# Nettiniilo ylläpitäjälle: *{{ book.abitti.nicename }}*

<!-- toc -->

## Yleistä Nettiniilon *{{ book.abitti.nicename }}*sta

Nettiniilon *{{ book.abitti.nicename }}* on tarkoitettu käytettäväksi oppilaitoksen arjessa ja esimerkiksi kurssikokeissa yhdessä YTL:n [Abitti-järjestelmän](http://www.abitti.fi/) kanssa.

*{{ book.abitti.nicename }}*ssa Nettiniilo toimii "kaapelinkorvaajana" mahdollistaen Abitti-järjestelmää hyödyntävien kurssikokeiden järjestämisen alkuperehdytyksen jälkeen ilman teknisen tuen tarvetta, kustannustehokkaasti ja ilman kaapeliviidakoita tai muita "johtotehtäviä".


## Teknistä tietoa moodista

Olleessaan *{{ book.abitti.nicename }}*ssa Nettiniilo on ethernet-verkon näkökulmasta kytkin (*{{ book.netti.nicename | lower }}*ssa Nettiniilo on reititin). Toisin sanoen, Nettiniilo ei *{{ book.abitti.nicename }}*ssa ollessaan toimi DHCP-palvelimena eikä siis jaa IP-osoitteita siihen langattomasti tai ethernet-kaapelilla liitetyille laitteille. Päinvastoin Nettiniilo olettaa *{{ book.abitti.nicename }}*ssa, että samassa verkossa on joku DHCP-palvelimen roolia toimittava laite. Abitti-koetilapalvelin on YTL:n toimesta ohjelmoitu toimimaan DHCP-palvelimena.

Nettiniilo tarjoaa hallintapaneelissaan ({{ book.abitti.urls.admin }}) määritetyn nimisen WLAN-verkon ja reitittää WLAN-liikenteen edelleen kuin kytkin.

Huomaa, että Nettiniilon hallintapaneeliin pääsee Abitti-palvelimelta muttei Abitti-opiskelijankoneelta; tämä rajoitus johtuu Abitti-järjestelmän palomuuriasetuksista.


## Mahdollisuus hybridiverkkoon

Oletusarvoisesti Nettiniiloa käytettäessä kaikki opiskelijat liittyvät Nettiniilon muodostamaan langattomaan verkkoon ja sitä kautta Abitti-koetilapalvelimeen. Nettiniilon avulla on kuitenkin mahdollista muodostaa myös hybridiverkko, jossa osa opiskelijoista liittyy verkkoon langattomasti ja osa ethernet-kaapelien kautta.


### Syitä hybridiverkon muodostamiseen

Hybridiverkon muodostaminen on varteenotettava vaihtoehto esimerkiksi jos

- osassa päätelaitteista langaton verkko ei syystä tai toisesta toimi Abitti-opiskelijantikun käyttöjärjestelmää käytettäessä tai
- halutaan liittää enemmän päätelaitteita samaan verkkoon kuin Nettiniilo jaksaa langattomasti palvella (Nettiniilon pitäisi pystyä palvelemaan *{{ book.abitti.nicename }}*ssa jopa 50-60 opiskelijaa yhtä aikaa).

### Hybridiverkon muodostaminen

Muodostaaksesi hybridiverkon tarvitset Nettiniilon ja Abitti-palvelimen lisäksi kytkimen (switch) sekä tietysti ethernet-kaapeleita. Huomaathan, että kytkin ja reititin ovat eri asia ja tässä tarvitaan nimenomaan kytkin.

![Abitti-verkko, jossa sekä langattomasti että kaapeleilla liittyneitä opiskelijoita](/images/abitti_hybridiverkko.png)

#### Hybridiverkon kytkentäohjeet

Toimi seuraavasti verkon muodostamiseksi:

1. Käynnistä Nettiniilo kytkemällä siihen virta
	- odota että WLAN-valo syttyy
	- varmista, että laite on *{{ book.abitti.nicename }}*ssa eli että WPS-valo palaa
2. Käynnistä Abitti-koetilapalvelin.
3. Liitä Nettiniilo PoE LAN -portistaan ethernet-johdolla kytkimeen.
4. Liitä Abitti-palvelin ethernet-johdolla kytkimeen.
5. Liitä ethernet-kaapelilla verkkoon liitettävät opiskelijoiden koneet kytkimessä vielä vapaana oleviin portteihin.



## Aineistojen jakaminen Nettiniilon avulla Abitti-kaapeliverkkoon

Nettiniiloa on mahdollista käyttää oheisaineistojen jakamiseen opiskelijoille siinäkin tapauksessa, että varsinaiset tietoliikenneyhteydet muodostetaan kaapeleilla, esim. atk-luokassa tai kielistudiossa.

Nettiniilon aineistonjako on nopea ja suoraviivainen käyttää:

1. Opettaja kopioi halutut tiedostot tavalliselle muistitikulle ja
2. liittää muistitikun Nettiniilon USB-porttiin.
3. Nyt jaopiskelijat näkevät Abitti-tikuilta käynnistetyillä koneillaan jaetut aineistot selaimellaan osoitteessa <{{ book.abitti.urls.share }}>

![Aineistonjako kaapeliverkossa Nettiniilon avulla](/images/abitti_aineistonjako-kaapeliverkkoon.png)

## WLAN-verkon käyttämän taajuuden/kanavan käsivalinta

Oletusarvoisesti Nettiniilon langaton verkko valitsee laitteen käynnistyksen yhteydessä käyttämäkseen liikennöintitaajuudeksi käynnistymishetkellä ko. tilassa mahdollisimman vähän käytetyn 2.4 GHz liikennöintialueella olevan WLAN-taajuuden/-kanavan.

On kuitenkin tilanteita, joissa on perusteltua asettaa Nettiniilo käyttämään aina samaa taajuutta/kanavaa. Näin esimerkiksi jos Nettiniilot asennetaan opetusluokkiin kiinteästi ja halutaan vierekkäisissä tiloissa olevat Nettiniilot käyttämään keskenään eri taajuuksia.

Taajuuden/kanavan manuaalivalinta on mahdollinen Nettiniilon hallintapaneelin *Paikallinen WLAN* -näkymän kautta Nettiniilon ohjelmistoversiosta v1.1.0 alkaen.



## Suorituskapasiteetti

Nettiniiloa on testattu valmistajan puolesta *{{ book.abitti.nicename }}*ssa enimmillään 60 yhtäaikaisesti Nettiniilon langattomaan verkkoon liittyneellä kannettavalla tietokoneella. Testaus suoritettiin Vaskivuoren lukiolla Vantaalla 25.4.2015.

- Abitti-palvelimena toimi tavallinen pöytäkone
- 60 Abitti-opiskelijantikuilta käynnistettyä langattomasti liittynyttä konetta
- Ylioppilastutkintolautakunnan kevyt kuormitustesti ok
- YTL:n raskas kuormitustesti hidastui 55 koneen kohdalla, mutta tämä saattoi myös johtua siitä, että palvelinkoneena oli vanha pöytäkone
- 255 kbit/s videon katsominen Nettiniilon materiaalinjaon kautta oppilaskoneille streamattuna
	- videon katselu aloitettiin pienellä porrastuksella
	- porrastus johtui siitä, että koneet piti "juosta läpi" play-nappia klikaten
	- 60 oppilaskoneessa verkon kapasiteetti alkoi tulla vastaan

### Yhteenveto

- Em. testeillä näyttäisi, että 50-60 langattomasti liittynyttä laitetta Abitti-verkossa on Nettiniilon suorituskyvyn maksimin tuntumassa.
- Huomaathan, että paikallinen 2.4GHz taajuuden "tukkoisuus" voi huonontaa saavutettavissa olevia tuloksia.
- Kannattaa seurata esim. Android-laitteille käytettävissä olevalla Wifi Analyzerilla taajuuksien käyttöä.
- Tarvittaessa Nettiniilo on ohjelmistoversiosta v1.1.0 alkaen mahdollista asettaa opettajille tarkoitetusta hallintapaneelista käsin käyttämään tiettyä taajuutta käynnistyksen yhteydessä tapahtuvan automaattivalinnan sijaan; tämä saattaa parantaa tuloksia tukkoisen 2.4GHz taajuuden tilanteessa esim. jos Nettiniilot asetetaan käyttämään "välikanavia" 3, 4, 8 tai 9.