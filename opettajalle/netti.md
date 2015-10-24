# Nettiniilon Nettimoodi opettajalle

## Yleistä Nettimoodista

Nettimoodi on tarkoitettu käytettäväksi silloin, kun halutaan käyttää opiskelijoiden omia päätelaitteita ilman YTL:n Abitti-järjestelmää. Nettiniilon nettimoodi mahdollistaa seuraavia asioita:

1. Mikäli Nettiniiloon on kytketty Internet-yhteys, on opettajalla mahdollisuus rajata yhteyttä oppituntikohtaisesti ja näin sallia pääsy vain haluttuihin verkkopalveluihin.
2. Opettaja näkee Nettiniilon tarjoamaan langattomaan verkkoon liittyneiden opiskelijoiden nimet.
3. Opettaja näkee verkossa käyneet, mutta siitä poistuneet opiskelijat.
4. Opettaja näkee verkossa käyneet, poistuneet ja takaisin tulleet opiskelijat.
5. Opettaja voi jakaa tiedostoja opiskelijoille Nettiniilon USB-porttiin liitetyltä muistitikulta.


## Nettiniilon käynnistäminen

Ottaaksesi Nettiniilon käyttöön nettimoodissa, toimi seuraavasti:

1. Irrota Nettiniilosta kaikki johdot.
2. Kytke pyöreäpäinen virtajohto Nettiniiloon.
3. Kytke virtajohdon toinen pää seinän virtaliittimeen.
4. Odota, että Nettiniilo käynnistyy.
	- Laite on valmis käytettäväksi kun laitteen etukannessa oleva WLAN-valo syttyy.
	- **HUOM!** Ennen 25.8.2015 toimitettujen Nettiniilojen mukana tulleissa ohjeissa kehotetaan odottamaan WPS-valon vilkkumisen päättymistä. Noudata kuitenkin yllä annettua ohjetta.
5. Varmista, että Nettiniilo on nettimoodissa:
	- Mikäli laitteen päällä oleva WPS-valo ei pala WLAN-valon sytyttyä, laite on jo nettimoodissa.
	- Mikäli laitteen päällä oleva WPS-valo palaa:
		- paina WPS-nappia kerran kevyesti (kuulet pienen napsahduksen) ja odota
		- parin sekunnin sisällä WPS-napin painamisesta nappi alkaa vilkkua
		- odota noin 10 sekuntia kunnes napin vilkkuminen päättyy
		- kun WPS-valo jää pois päältä, on laite nettimoodissa
6. Jatka ohjeiden seuraavaan vaiheeseen.

![Kuva tai video Nettiniilon käynnistämisestä](http://placehold.it/600x300 "Kuva tai video Nettiniilon käynnistämisestä")


## Yhteys Nettiniilon ja opettajan koneen välille

Kun olet käynnistänyt Nettiniilon, toimi seuraavasti liittääksesi käyttämäsi koneen Nettiniiloon sen hallinnointia varten:

1. Varmista, että olet käynnistänyt Nettiniilon ja että se on nettimoodissa.
4. Käynnistä oma koneesi ja kytke ethernet-johto koneesi ethernet-portista Nettiniilon PoE LAN -porttiin.
5. Jatka ohjeiden seuraavaan vaiheeseen.

### Verkkokaavio

![Verkkokaavio](http://placehold.it/600x300 "Verkkokaavio")


## Nettiniilon hallintapaneeliin kirjautuminen nettimoodissa

Nyt kun olet käynnistänyt Nettiniilon, asettanut sen nettimoodiin ja liittänyt koneesi ethernet-johdolla Nettiniilon PoE LAN -porttiin, voit jatkaa seuraavaan vaiheeseen eli kirjautua sisään Nettiniilon hallintapaneeliin:

1. Avaa Chrome- tai Firefox-selaimella uusi välilehti painamalla `Ctrl+T` (Apple: `Command+T`)
2. Mene selainikkunassa seuraavaan osoitteeseen: <{{ book.netti.urls.admin }}>
3. Nyt sinulle pitäisi aueta kaavake, jossa saatetietona lukee *Nettiniilon hallinta* ja sinua pyydetään syöttämään käyttäjätunnus ja salasana Nettiniilon hallintapaneeliin kirjautuaksesi.
4. Syötä laitteen mukana toimitettuihin ohjeisiin kirjattu käyttäjätunnus ja salasana laitteen.
	- Huomioithan, että salasana voi olla myös muutettu tehdasasetuksista
	- Hallintapaneeliin käyttäjätunnus ja salasana eivät muutu Nettiniilon moodia vaihdettaessa

![Nettiniilon hallintapaneeliin kirjautuminen](http://placehold.it/600x300 "Nettiniilon hallintapaneeliin kirjautuminen")

### Huomioita hallintapaneeliin kirjautumisesta

- Hallintapaneeli toimii parhaiten Chrome- ja Firefox-selaimilla.
	- Tiedossa on, että Internet Explorer -selaimella hallintapaneeli ei välttämättä toimi oikein.
- Halutessasi kirjautua hallintapaneeliin, älä kirjoita osoitetta <{{ book.netti.urls.admin }}> selaimen mahdolliseen hakukenttään ruudun pystysuunnassa keskelle vaan selaimen yläreunassa olevaan osoitekenttään. Paina tämä jälkeen `Enter`.


## WLAN-verkon nimen ja salasanan tarkistaminen/asettaminen

Nyt kun olet kirjautunut Nettiniilon hallintapaneeliin, toimi seuraavasti:

1. Mene Nettiniilon hallintapaneelissa *Paikallinen WLAN* -välilehdelle.
2. Varmista, että *Tukiaseman nimi* ja *WLAN-salasana* (tai *WLAN-suojausavain*) -kohdissa on haluamasi asetukset.
3. Mikäli
	- et halua muuttaa asetuksia, näet nykyiset WLAN-verkkoon liittymiseen tarvittavat tiedot.
	- haluat muuttaa asetuksia, kirjoita kenttiin haluamasi tiedot ja paina *Tallenna*-nappia.
	- haluat tehdä rajauksia Internet-yhteyteen ennenkuin opiskelijat liittyvät verkkoon, älä kerro WLAN-verkon salasanaa opiskelijoille vielä.

![WLAN-verkon nimi ja salasana](http://placehold.it/600x300 "WLAN-verkon nimi ja salasana")

### Huomioita WLAN-verkon nimen asettamisesta

Opettaja, mikäli vaihdoit WLAN-verkon nimeä edellä ja mikäli opiskelijoilla oli jo siinä vaiheessa koneet käynnistettynä, kestää opiskelijankoneilla yleensä noin 10-20 sekuntia tajuta, että Nettiniilon tarjoaman verkon nimi on muuttunut. Tänä aikana opikelijan WLAN-verkkoon liittymisen valikossa saattaa hetkellisesti näkyä sekä vanha että uusi verkon nimi tai ei kumpaakaan.



## Internet-yhteyden muodostaminen Nettiniilosta

### Internet-yhteys ethernet-kaapelilla koulun seinään

### Internet-yhteys mokkulan kautta


## Sallittujen Internet-osoitteiden asettaminen


## Opiskelijoiden ohjeistaminen Nettiniilon WLAN-verkkoon liittymiseen

Kun olet opettajana tehnyt tarvittavat asetukset Nettiniilon hallintapaneelissa, toisin sanoen vaihtanut WLAN-verkon nimeä ja/tai salasanaa, muodostanut Internet-yhteyden Nettiniilosta eteenpäin ja halutessasi asettanut Internet-yhteyden osoiterajaukset, olet nyt valmis ohjeistamaan opiskelijoita liittymään Nettiniilon tarjoamaan langattomaan verkkoon.

Ohjeista opiskelijoita seuraavasti:

1. Kerro opiskelijoille Nettiniilon tarjoaman WLAN-verkon nimi ja salasana.
2. Ohjeista opiskelijoita liittymään em. langattomaan verkkoon **porrastetusti**
	- yksi liittyjä per noin 1-2 sekuntia
	- ts. 30 opiskelijan ryhmän tulisi käyttää liittymiseen porrastetusti 30-60 sekuntia
3. Opiskelijoiden on verkkoon liittymisensä jälkeen vielä rekisteröidyttävä syöttämällä etu- ja sukunimensä.
	- Ohjeista opiskelijoita menemään selaimellaan osoitteeseen <{{ book.netti.urls.landing }}> rekisteröityäkseen.
	- Rekisteröitymisen jälkeen opiskelijoilla on pääsy Nettiniilon materiaalinjakoon (<{{ book.netti.urls.share }}>).
	- Mikäli Nettiniilosta on Internet-yhteys eteenpäin, on opiskelijoilla nyt pääsy Internetiin.

<!--
* Jos koulun koneilla käytössä proxy- eli välityspalvelin, on se otettava koneelta pois päältä, jotta Nettiniilon Netti-moodia voi käyttää
* Ohjeista hallintapaneeliin meno aina <{{ book.netti.urls.admin }}>, ei http://nettiniilo.lan
-->