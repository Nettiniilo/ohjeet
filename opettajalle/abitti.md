# Nettiniilon Abitti-moodi opettajalle

## Yleistä Abitti-moodista

Nettiniilon Abitti-moodi on tarkoitettu käytettäväksi oppilaitoksen arjessa ja esimerkiksi kurssikokeissa yhdessä Ylioppilastutkintolautakunnan [Abitti-järjestelmän](http://www.abitti.fi/) kanssa.

Nettiniilo toimii "kaapelinkorvaajana" mahdollistaen Abitti-järjestelmää hyödyntävien kurssikokeiden järjestämisen alkuperehdytyksen jälkeen minimaalisella teknisellä tuella, kustannustehokkaasti ja ilman kaapeliviidakoita tai muita "johtotehtäviä".


## Nettiniilon käynnistäminen

Ottaaksesi Nettiniilon käyttöön Abitti-järjestelmän kanssa käytettäväksi, toimi seuraavasti:

1. Irrota Nettiniilosta kaikki johdot.
2. Kytke pyöreäpäinen virtajohto Nettiniiloon.
3. Kytke virtajohdon toinen pää seinän virtaliittimeen.
4. Odota, että Nettiniilo käynnistyy.
	- Laite on valmis käytettäväksi kun laitteen etukannessa oleva WLAN-valo syttyy.
	- **HUOM!** Ennen 25.8.2015 toimitettujen Nettiniilojen mukana tulleissa ohjeissa kehotetaan odottamaan WPS-valon vilkkumisen päättymistä. Noudata kuitenkin yllä annettua ohjetta.
5. Varmista, että Nettiniilo on Abitti-moodissa:
	- Mikäli laitteen päällä oleva WPS-valo palaa, laite on jo Abitti-moodissa.
	- Mikäli laitteen päällä oleva WPS-valo ei pala:
		- paina WPS-nappia kerran kevyesti (kuulet pienen napsahduksen) ja odota
		- parin sekunnin sisällä WPS-napin painamisesta nappi alkaa vilkkua
		- odota noin 10 sekuntia kunnes napin vilkkuminen päättyy
		- kun WPS-valo jää palamaan, on laite Abitti-moodissa
6. Jatka ohjeiden seuraavaan vaiheeseen.

![Kuva tai video Nettiniilon käynnistämisestä](http://placehold.it/600x300 "Kuva tai video Nettiniilon käynnistämisestä")

## Koetilapalvelimen käynnistäminen

Abitti-järjestelmän käyttämistä varten tarvitset Abitti-koetilapalvelimen.

1. Mikäli käytät koetilapalvelimena konetta, jossa ei ole ethernet-porttia ja joudut näin ollen käyttämään USB-ethernet-sovitinta (esim. Applen Macbook Air -kannettavat), varmista että USB-ethernet-sovitin on kytkettynä koneeseen ennen seuraavaan vaiheeseen siirtymistä.
2. Käynnistä opettajan koneesi Abitti-koetilapalvelimeksi Abitti-koetilapalvelinmuistitikulta.
3. Jatka ohjeiden seuraavaan vaiheeseen.

## Yhteys Nettiniilon ja koetilapalvelimen välille

Jotta opiskelijoiden Abitti-muistitikuilta käynnistetyt koneet voivat kommunikoida Abitti-koetilapalvelimen kanssa, on niiden välille muodostettava tietoliikenneyhteydet. Nettiniilon avulla tarvittavien tietoliikenneyhteyksien luominen on vaivatonta.

1. Varmista, että olet käynnistänyt Nettiniilon ja että se on Abitti-moodissa.
4. Kun koetilapalvelin on käynnistynyt, kytke ethernet-johto koetilapalvelimesta Nettiniilon PoE LAN -porttiin.
5. Jatka ohjeiden seuraavaan vaiheeseen.

### Verkkokaavio

![Verkkokaavio](http://placehold.it/600x300 "Verkkokaavio")

### Verkon muodostamisen ohjevideo

![Kuva tai video verkon muodostamisesta](http://placehold.it/600x300 "Kuva tai video verkon muodostamisesta")

## Nettiniilon hallintapaneeliin kirjautuminen Abitti-moodissa

Nyt kun olet käynnistänyt Nettiniilon, asettanut sen Abitti-moodiin, käynnistänyt Abitti-koetilapalvelimen ja liittänyt koetilapalvelimen ethernet-johdolla Nettiniilon PoE LAN -porttiin, voit jatkaa seuraavaan vaiheeseen eli kirjautua sisään Nettiniilon hallintapaneeliin Abitti-koetilapalvelimelta:

1. Avaa koetilapalvelimen {{ book.abitti.browser }}-selainohjelmassa uusi välilehti painamalla `Ctrl+T`.
2. Mene selainikkunassa seuraavaan osoitteeseen: <{{ book.abitti.urls.admin }}>
3. Nyt sinulle pitäisi aueta kaavake, jossa saatetietona lukee *Nettiniilon hallinta* ja sinua pyydetään syöttämään käyttäjätunnus ja salasana Nettiniilon hallintapaneeliin kirjautuaksesi.
4. Syötä laitteen mukana toimitettuihin ohjeisiin kirjattu käyttäjätunnus ja salasana laitteen.
	- Huomioithan, että salasana voi olla myös muutettu tehdasasetuksista
	- Hallintapaneeliin käyttäjätunnus ja salasana eivät muutu Nettiniilon moodia vaihdettaessa

![Nettiniilon hallintapaneeliin kirjautuminen](http://placehold.it/600x300 "Nettiniilon hallintapaneeliin kirjautuminen")

### Huomioita hallintapaneeliin kirjautumisesta

- Hallintapaneeli toimii parhaiten Chrome- ja Firefox-selaimilla.
	- Abitti-koetilapalvelimessa on oletuksena käytössä {{ book.abitti.browser }}-selain, joka on käytännössä Firefox muutamia eroavaisuuksia lukuunottamatta.
	- Tiedossa on, että Internet Explorer -selaimella hallintapaneeli ei välttämättä toimi oikein. Tämä ei ole ongelma Abitti-moodissa, mutta Netti-moodissa kylläkin.
- Jotta hallintapaneeliin meneminen onnistuu 17.8.2015 jälkeen päivitetyllä Abitti-palvelintikulla (Abitti-palvelintikun v37 tai uudempi), on Nettiniilon ohjelmistoversion oltava vähintään v1.0.0!* Mikäli näin ei ole, päivitä Nettiniilo ensin Netti-moodissa!
- Halutessasi kirjautua hallintapaneeliin, älä kirjoita osoitetta <{{ book.abitti.urls.admin }}> selaimen mahdolliseen hakukenttään ruudun pystysuunnassa keskelle vaan selaimen yläreunassa olevaan osoitekenttään. Paina tämä jälkeen `Enter`.


## WLAN-verkon nimen ja salasanan tarkistaminen/asettaminen

Nyt kun olet kirjautunut Abitti-palvelimen {{ book.abitti.browser }}-selaimen avulla Nettiniilon hallintapaneeliin, toimi seuraavasti:

1. Mene Nettiniilon hallintapaneelissa *Paikallinen WLAN* -välilehdelle.
2. Varmista, että *Tukiaseman nimi* ja *WLAN-salasana* (tai *WLAN-suojausavain*) -kohdissa on haluamasi asetukset.
3. Mikäli
	- et halua muuttaa asetuksia, kerro kentissä näkyvät tiedot opiskelijoille.
	- haluat muuttaa asetuksia, kirjoita kenttiin haluamasi tiedot ja paina *Tallenna*-nappia.
4. Opiskelijat voivat nyt liittyä Abitti-muistitikuilta käynnistetyillä koneillaan Nettiniilon tarjoamaan langattomaan verkkoon ja saavat sitä kautta yhteyden Abitti-koetilapalvelimeen.
	- Abitti-opiskelijantikulta käynnistetyllä tietokoneella langattomaan verkkoon liittyminen onnistuu ruudun oikeasta ylänurkasta kellonajan vierestä.
	- Opiskelija klikkaa kuvaketta, jossa näkyy <!-- todo --> ikäänkuin kaksi sinistä tietokoneen ruutua ja valkoinen raksi punaisella pohjalla.
	- Tämän jälkeen opiskelija valitsee opettajan kertoman WLAN-verkon nimen ja syöttää opettajan kertoman salasanan.

![WLAN-verkon nimi ja salasana](http://placehold.it/600x300 "WLAN-verkon nimi ja salasana")

### Huomioita WLAN-verkon nimen asettamisesta

Opettaja, mikäli vaihdoit WLAN-verkon nimeä edellä ja mikäli opiskelijoilla oli jo siinä vaiheessa koneet käynnistettynä Abitti-opiskelijantikuilta, kestää opiskelijankoneilla yleensä noin 10-20 sekuntia tajuta, että Nettiniilon tarjoaman verkon nimi on muuttunut. Tänä aikana opikelijan WLAN-verkkoon liittymisen valikossa saattaa hetkellisesti näkyä sekä vanha että uusi verkon nimi tai ei kumpaakaan.

## Loppusilaus ja sitten on valmista!

Nyt sinulla on Abitti-verkko valmiina käyttöön. Tee vielä seuraavat toimet niin voitte aloittaa Abitti-järjestelmän käytön opiskelijoiden kanssa:

1. Lataa koepaketti [oma.abitti.fi](https://oma.abitti.fi)-palvelusta muistitikulle eli nk. *siirtotikulle*.
2. Liitä muistitikku Abitti-koetilapalvelimen roolia toimittavaan koneeseen.
3. Valitse koetilapalvelimella käyttöön siirtotikulle tallentamasi koetiedosto ja syötä oma.abitti.fi-palvelusta tiedostoa varten saamasi purkuavain.
4. Nyt pääsette aloittamaan sähköisen kokeen!

![Kuva tai video koepaketin tuonnista käyttöön](http://placehold.it/600x300 "Kuva tai video koepaketin tuonnista käyttöön")

## Lisämahdollisuudet

Abitti-järjestelmän kanssa käytettäessä Nettiniilo toimii minimissään *"kaapelinkorvaajana"*. Perustoiminnallisuuden lisäksi Nettiniilo tarjoaa kuitenkin seuraavia lisämahdollisuuksia Abitti-käyttöä monipuolistamaan.

### Tiedostojenjako

Nettiniilo tarjoaa opettajalle mahdollisuuden jakaa oheisaineistoja opiskelijoiden käyttöön esimerkiksi Abitti-kokeen oheisaineistoksi. Oheisaineistoina voidaan käyttää kaikkia Abitti-opiskelijankoneella avattavissa olevia tiedostotyyppejä; näitä ovat mm. seuraavat:

- Microsoft Office -tiedostot
	- Word-tiedostot (.docx ja .doc)
	- Excel-tiedostot (.xlsx ja .xls)
	- Powerpoint-tiedostot (.pptx ja .ppt)
- LibreOffice-tiedostot
- PDF-tiedostot (.pdf)
- Kuvatiedostot (muun muassa: .png, .jpg, .gif, .svg, .psd, .xcf)
- GeoGebra-tiedostot (.ggb)
- Äänitiedostot (.mp3, .wav, .ogg)
- Videotiedostot (.mp4, .avi, .mov, .webm, .ogv)

#### Huomio YTL:n toimien vaikutuksesta aineistonjakoon

Huomaathan, että oheisaineistojen eri tiedostotyyppien avautuvuus suoraan selaimessa ja toisaalta toimivuus ylipäätään Abitti-opiskelijankoneilla on kiinni Ylioppilastutkintolautakunnan Abitti-opiskelijantikuille sisällyttämistä ohjelmista ja niiden asetuksista.

#### Tiedostojen jakaminen opiskelijoille

Tiedostoja jaetaan opiskelijoille tallentamalla jaettavaksi halutut tiedostot omalla tietokoneella tavalliselle muistitikulle ja liittämällä tämän jälkeen kyseinen muistitikku Nettiniilon USB-porttiin.

#### Tiedostojenjaon osoite Abitti-moodissa

Abitti-moodissa opiskelijat pääsevät tarkastelemaan tiedostojenjaossa tarjolla olevaa aineistoa osoitteessa:
<{{ book.abitti.urls.share }}> . Huomaa, että Abitti-koetilapalvelimelta ei ole pääsyä kyseiseen osoitteeseen koetilapalvelimen osoiterajauksista johtuen.

#### Ei skandeja ja lainausmerkkejä tiedostonimiin

Huomaa, että tiedostoja opiskelijoille Nettiniilon kautta jaettaessa älä käytä tiedostonimissä ääkkösiä äläkä lainausmerkkejä; mikäli tiedostonimi sisältää em. merkkejä, ei opiskelija pysty käyttämään tiedostoa! Syy on tiedossa ja korjaus tehtävälistalla, mutta korjaus ei ole prioriteettilistan kärjessä.


### Tiedostojen palautus

Nettiniilon ohjelmistopäivityksen version 1.1 myötä opiskelijat voivat myös palauttaa tiedostoja opettajalle menemällä Abitti-järjestelmäään käynnistetyllä selaimellaan tiedostojenpalautuksen osoitteeseen: <{{ book.abitti.urls.upload }}>

Näin ollen Abitti-kokeissa on mahdollista toteuttaa laajempia kysymystyyppejä kun vastaukset eivät ole rajoitettuja Abitti-järjestelmän tarjoamiin pelkkiin tekstivastauksiin.

#### Tiedostojenpalautukseen ei pääsyä koetilapalvelimelta

Huomaa, että opettajan koetilapalvelimelta ei ole koetilapalvelimen palomuuriasetuksista johtuen pääsyä tiedostojenpalautuksen mukaiseen osoitteeseen (<{{ book.abitti.urls.upload }}>) vaikka opiskelijoiden Abitti-järjestelmään käynnistetyiltä koneilta kyseiseen osoitteseen onkin pääsy.