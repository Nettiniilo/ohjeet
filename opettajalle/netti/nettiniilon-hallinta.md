# Nettiniilon hallinta (*{{ book.netti.nicename }}*)

## Hallintapaneeliin kirjautuminen

Nyt kun olet käynnistänyt Nettiniilon, asettanut sen *{{ book.netti.nicename }}*in ja liittänyt koneesi ethernet-johdolla Nettiniilon PoE LAN -porttiin, voit jatkaa seuraavaan vaiheeseen eli kirjautua sisään Nettiniilon hallintapaneeliin:

1. Avaa Chrome- tai Firefox-selaimella uusi välilehti painamalla `Ctrl+T` (Apple: `Command+T`)
2. Mene selainikkunassa seuraavaan osoitteeseen: <{{ book.netti.urls.admin }}>
3. Nyt sinulle pitäisi aueta kaavake, jossa saatetietona lukee *Nettiniilon hallinta* ja sinua pyydetään syöttämään käyttäjätunnus ja salasana Nettiniilon hallintapaneeliin kirjautuaksesi.
4. Syötä laitteen mukana toimitettuihin ohjeisiin kirjattu käyttäjätunnus ja salasana laitteen.
	- Huomioithan, että salasana voi olla myös muutettu tehdasasetuksista
	- Hallintapaneeliin käyttäjätunnus ja salasana eivät muutu Nettiniilon moodia vaihdettaessa

![Nettiniilon hallintapaneeliin kirjautuminen](http://placehold.it/800x400 "Nettiniilon hallintapaneeliin kirjautuminen (tulossa)")

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

![WLAN-verkon nimi ja salasana](http://placehold.it/800x400 "WLAN-verkon nimi ja salasana (tulossa)")

### Huomioita WLAN-verkon nimen asettamisesta

Opettaja, mikäli vaihdoit WLAN-verkon nimeä edellä ja mikäli opiskelijoilla oli jo siinä vaiheessa koneet käynnistettynä, kestää opiskelijankoneilla yleensä noin 10-20 sekuntia tajuta, että Nettiniilon tarjoaman verkon nimi on muuttunut. Tänä aikana opikelijan WLAN-verkkoon liittymisen valikossa saattaa hetkellisesti näkyä sekä vanha että uusi verkon nimi tai ei kumpaakaan.

## Internet-yhteyden muodostaminen Nettiniilosta

Nettiniilo on mahdollista yhdistää Internetiin joko ethenet-kaapelilla tai 3G/4G-yhteydellä mokkulan kautta. Tämän jälkeen on mahdollista tarjota opiskelijoille Internet-yhteys Nettiniilon WLAN-verkon kautta. Tällöin opettajalle tarjoutuu mahdollisuus a) rajata niitä sivustoja, joihin opiskelijoilla on pääsy ja b) jakaa opiskelijoille oheisaineistoja Nettiniilon kautta.

### Internet-yhteys ethernet-kaapelilla koulun seinään

VAROITUS: Mikäli Internet-yhteys halutaan muodostaa liittämällä Nettiniilo oppilaitoksen olemassaolevaan tietoverkkoon (ethernet-kaapelilla seinään), täytyy tähän ehdottomasti olla *rehtorin/tietohallinnon lupa*!

Kun olet saanut luvan liittää Nettiniilon oppilaitoksenne Internet-yhteyteen (seinäliittimeen) ethernet-kaapelilla, toimi seuraavasti:

1. Varmista, että Nettiniilo on käynnistetty ja *{{ book.netti.nicename }}*ssa.
2. Yhdistä ethernet-kaapeli Nettiniilon *WAN/LAN-portista* todennäköisimmin seinässä olevaan ethernet-pistokeeseen.
	- VAROITUS: Älä kytke ethernet-johtoa Nettiniilon *PoE LAN -portista* seinään!

### Internet-yhteys mokkulan kautta

Tulossa...

## Sallittujen Internet-osoitteiden asettaminen

Tulossa...

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
* Jos koulun koneilla käytössä proxy- eli välityspalvelin, on se otettava koneelta pois päältä, jotta Nettiniilon *{{ book.netti.nicename }}*a voi käyttää
* Ohjeista hallintapaneeliin meno aina <{{ book.netti.urls.admin }}>, ei http://nettiniilo.lan
-->