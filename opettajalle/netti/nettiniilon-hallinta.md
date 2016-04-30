# Nettiniilon hallinta (*{{ book.netti.nicename | lower }}*)

<!-- toc -->

## Hallintapaneeliin kirjautuminen

Nyt kun olet käynnistänyt Nettiniilon, asettanut sen *{{ book.netti.nicename | lower }}*in ja liittänyt koneesi ethernet-johdolla Nettiniilon PoE LAN -porttiin, voit jatkaa seuraavaan vaiheeseen eli kirjautua sisään Nettiniilon hallintapaneeliin:

1. Avaa Chrome- tai Firefox-selaimella uusi välilehti painamalla `Ctrl+T` (Apple: `Command+T`)
2. Mene selainikkunassa seuraavaan osoitteeseen: <{{ book.netti.urls.admin }}>
3. Nyt sinulle pitäisi aueta kaavake, jossa saatetietona lukee *Nettiniilon hallinta* ja sinua pyydetään syöttämään käyttäjätunnus ja salasana Nettiniilon hallintapaneeliin kirjautuaksesi.
4. Syötä laitteen mukana toimitettuihin ohjeisiin kirjattu käyttäjätunnus ja salasana laitteen.
	- Huomioithan, että salasana voi olla myös muutettu tehdasasetuksista
	- Hallintapaneeliin käyttäjätunnus ja salasana eivät muutu Nettiniilon moodia vaihdettaessa

### Huomioita hallintapaneeliin kirjautumisesta

- Hallintapaneeli toimii parhaiten Chrome- ja Firefox-selaimilla.
	- Tiedossa on, että Internet Explorer -selaimella hallintapaneeli ei välttämättä toimi oikein.
- Halutessasi kirjautua hallintapaneeliin, älä kirjoita osoitetta <{{ book.netti.urls.admin }}> selaimen mahdolliseen hakukenttään ruudun pystysuunnassa keskelle vaan selaimen yläreunassa olevaan osoitekenttään. Paina tämä jälkeen *Enter*.



## WLAN-verkon nimen ja salasanan tarkistaminen/asettaminen

Nyt kun olet kirjautunut Nettiniilon hallintapaneeliin, toimi seuraavasti:

1. Mene Nettiniilon hallintapaneelissa *Paikallinen WLAN* -välilehdelle.
2. Varmista, että *Tukiaseman nimi* ja *WLAN-salasana* (tai *WLAN-suojausavain*) -kohdissa on haluamasi asetukset.
3. Mikäli
	- et halua muuttaa asetuksia, näet nykyiset WLAN-verkkoon liittymiseen tarvittavat tiedot.
	- haluat muuttaa asetuksia, kirjoita kenttiin haluamasi tiedot ja paina *Tallenna*-nappia.
	- haluat tehdä rajauksia Internet-yhteyteen ennenkuin opiskelijat liittyvät verkkoon, älä kerro WLAN-verkon salasanaa opiskelijoille vielä.

![Nettiniilon opiskelijoille tarjoaman WLAN-verkon nimi ja salasana](/images/nettimoodi_paikallinen-wlan.png)

### Huomioita WLAN-verkon nimen asettamisesta

Opettaja, mikäli vaihdoit WLAN-verkon nimeä edellä ja mikäli opiskelijoilla oli jo siinä vaiheessa koneet käynnistettynä, kestää opiskelijankoneilla yleensä noin 10-20 sekuntia tajuta, että Nettiniilon tarjoaman verkon nimi on muuttunut. Tänä aikana opikelijan WLAN-verkkoon liittymisen valikossa saattaa hetkellisesti näkyä sekä vanha että uusi verkon nimi tai ei kumpaakaan.



## Internet-yhteyden muodostaminen Nettiniilosta

Nettiniilo on mahdollista yhdistää Internetiin joko ethenet-kaapelilla tai vaihtoehtoisesti mokkulan tai USB-kaapelilla Nettiniiloon liitetyn kännykän kautta. Huomaa, että 4G-mokkulan ja kännykän käyttämiseksi Internet-yhteyden muodostamiseen tarvitaan vähintään Nettiniilon ohjelmistoversio v1.1.0.

Kun Internet-yhteys on muodostesttu Nettiniilosta eteenpäin, on tämän jälkeen on mahdollista tarjota opiskelijoille Internet-yhteys Nettiniilon jakaman WLAN-verkon kautta. Tällöin opettajalle tarjoutuu mahdollisuus a) rajata niitä sivustoja, joihin opiskelijoilla on pääsy ja b) jakaa opiskelijoille oheisaineistoja Nettiniilon kautta.

![Internet-yhteyden muodostaminen Nettiniilosta eteenpäin](/images/nettimoodi_internet-yhteys.png)

### Internet-yhteys ethernet-kaapelilla koulun seinään

VAROITUS: Mikäli Internet-yhteys halutaan muodostaa liittämällä Nettiniilo oppilaitoksen olemassaolevaan tietoverkkoon (ethernet-kaapelilla seinään), täytyy tähän ehdottomasti olla *rehtorin/tietohallinnon lupa*!

Kun olet saanut luvan liittää Nettiniilon oppilaitoksenne Internet-yhteyteen (seinäliittimeen) ethernet-kaapelilla, toimi seuraavasti:

1. Varmista, että Nettiniilo on käynnistetty ja *{{ book.netti.nicename | lower }}*ssa.
2. Yhdistä ethernet-kaapeli Nettiniilon *WAN/LAN-portista* todennäköisimmin seinässä olevaan ethernet-pistokeeseen.
	- VAROITUS: Älä kytke ethernet-johtoa Nettiniilon *PoE LAN -portista* seinään!

### Internet-yhteys 3G-mokkulan kautta

Ainakin seuraavat 3G-mokkulamallit toimivat Nettiniilon kanssa: Huawei E220, E353, E367 ja E3131. Näitä mokkulamalleja käytettäessä toimi seuraavasti:

0. Älä liitä mokkulaa Nettiniilon USB-porttiin ennen alla kerrottujen asetusten tekemistä.
1. Aseta käyttämäsi SIM-kortin operaattorin vaatima APN-tieto *APN*-kenttään:
	- DNA, Elisa ja Sonera: `internet`
	- Saunalahti: `internet.saunalahti`
2. Aseta mokkulassa sisällä olevan SIM-kortin PIN-koodi.
3. Paina *Tallenna*-nappia.
4. Liitä 3G-mokkula Nettiniilon USB-porttiin.
5. Odota arviolta vajaa minuutti yhteyden muodostumista.

### Internet-yhteys 4G-mokkulan kautta

Huawei E3372 -mallisella 4G-mokkulalla Internet-yhteys toimii Nettiniilon ohjelmistoversiosta v1.1.0 alkaen suoraan kun mokkulan yksinkertaisesti kytkee Nettiniilon USB-porttiin. Muita 4G-mokkuloita ei ole testattu Nettiniilon kanssa.

### Internet-yhteys kännykän ja USB-johdon avulla

Internet-yhteyden jakaminen kännykästä USB-johdon kautta Nettiniilon vaatii vähintään Nettiniilon ohjelmistoversion v1.1.0. Kännykästä nettiyhteyden jakaminen toimii ainakin Android 4 ja Android 5 -kännyköissä. Toimi seuraavasti:

1. Liitä kännykkä USB-johdolla Nettiniilon USB-porttiin.
2. Aseta kännykässä USB-portin kautta tapahtuva nettiyhteyden jako päälle (USB tethering).
3. Nettiniilossa ei tarvitse varsinaisesti tehdä mitään.


## Sallittujen Internet-osoitteiden asettaminen

Varmista, että Nettiniilo on liitettynä Internet-yhteyteen joko WAN/LAN-portin kautta ethernet-kaapelilla tai vaihtoehtoisesti mokkulan tai kännykän kautta. Tämän jälkeen toimi Nettiniilon hallintapaneelissa ({{ book.netti.urls.admin }}) seuraavasti:

1. Mene hallintapaneelissa *Sallitut domainit* -näkymään.
2. Tarkista liittyykö sallituiksi haluamiisi Internet-sivustoihin joitakin erityisohjeita klikkaamalla *[Ohjeita tiettyjen palvelujen sallimiseen](osoiterajaus.html)* -linkkiä
3. Syötä sallituksi haluamasi domainit *Sallitut domainit* -kenttään, yksi domain per rivi. Rajaus toimii whitelist-pohjaisesti eli osoitteet, joita ei ole sallittu, ovat estettyjä.
4. Voit sallia useampia verkkopalveluita listaamalla tarvittavat domainit, yksi per rivi.
5. Kun olet syöttänyt haluamasi domainit ja niihin [lisäohjeissa](osoiterajaus.html) mahdollisesti kehotetut lisädomainit, paina *Aloita rajaus* -nappia.

![Sallittujen domainien asettaminen Nettiniilon hallintapaneelissa {{ book.netti.nicename | lower}}ssa.](/images/nettimoodi_sallitut-domainit.png)



## Opiskelijoiden ohjeistaminen Nettiniilon WLAN-verkkoon liittymiseen

Kun olet opettajana tehnyt tarvittavat asetukset Nettiniilon hallintapaneelissa, toisin sanoen vaihtanut WLAN-verkon nimeä ja/tai salasanaa, muodostanut Internet-yhteyden Nettiniilosta eteenpäin ja halutessasi asettanut Internet-yhteyden osoiterajaukset, olet nyt valmis ohjeistamaan opiskelijoita liittymään Nettiniilon tarjoamaan langattomaan verkkoon.

Ohjeista opiskelijoita seuraavasti:

1. Kerro opiskelijoille Nettiniilon tarjoaman WLAN-verkon nimi ja salasana.
2. Ohjeista opiskelijoita liittymään em. langattomaan verkkoon **porrastetusti**
	- käyttäkää vähintään muutamia sekunteja per verkkoon liittyjä, esim. 3-5 sekuntia
	- ts. 30 opiskelijan ryhmän tulisi käyttää liittymiseen porrastetusti muutaman minuutin aikajänteellä
3. Opiskelijoiden on verkkoon liittymisensä jälkeen vielä rekisteröidyttävä syöttämällä etu- ja sukunimensä.
	- Ohjeista opiskelijoita menemään selaimellaan osoitteeseen <{{ book.netti.urls.landing }}> rekisteröityäkseen.
	- Rekisteröitymisen jälkeen opiskelijoilla on pääsy Nettiniilon materiaalinjakoon (<{{ book.netti.urls.share }}>).
	- Mikäli Nettiniilosta on Internet-yhteys eteenpäin, on opiskelijoilla nyt pääsy Internetiin.

<!--
* Jos koulun koneilla käytössä proxy- eli välityspalvelin, on se otettava koneelta pois päältä, jotta Nettiniilon *{{ book.netti.nicename | lower }}*a voi käyttää
* Ohjeista hallintapaneeliin meno aina <{{ book.netti.urls.admin }}>, ei http://nettiniilo.lan
-->