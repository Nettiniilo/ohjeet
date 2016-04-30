# Nettiniilon hallinta (*{{ book.abitti.nicename }}*)

## Kirjautuminen Nettiniiloon

Nyt kun olet käynnistänyt Nettiniilon, asettanut sen *{{ book.abitti.nicename }}*in, käynnistänyt Abitti-koetilapalvelimen ja liittänyt koetilapalvelimen ethernet-johdolla Nettiniilon PoE LAN -porttiin, voit jatkaa seuraavaan vaiheeseen eli kirjautua sisään Nettiniilon hallintapaneeliin Abitti-koetilapalvelimelta:

1. Avaa koetilapalvelimen {{ book.abitti.browser }}-selainohjelmassa uusi välilehti painamalla `Ctrl+T`.
2. Mene selainikkunassa seuraavaan osoitteeseen: <{{ book.abitti.urls.admin }}>
3. Nyt sinulle pitäisi aueta kaavake, jossa saatetietona lukee *Nettiniilon hallinta* ja sinua pyydetään syöttämään käyttäjätunnus ja salasana Nettiniilon hallintapaneeliin kirjautuaksesi.
4. Syötä laitteen mukana toimitettuihin ohjeisiin kirjattu käyttäjätunnus ja salasana laitteen.
	- Huomioithan, että salasana voi olla myös muutettu tehdasasetuksista
	- Hallintapaneeliin käyttäjätunnus ja salasana eivät muutu Nettiniilon moodia vaihdettaessa

<div class="video-container-4by3" style="position:relative; padding-bottom:71.2%; padding-top:30px; height:0; overflow:hidden;">
<iframe style="position:absolute; top:0; left:0; width:100%; height:100%;" width="420" height="315" src="https://www.youtube.com/embed/Ll5rfAPH0oA" frameborder="0" allowfullscreen></iframe>
</div>

<!-- ![Nettiniilon hallintapaneeliin kirjautuminen](https://placehold.it/800x400 "Nettiniilon hallintapaneeliin kirjautuminen (tulossa)") -->

### Huomioita hallintapaneeliin kirjautumisesta

- Hallintapaneeli toimii parhaiten Chrome- ja Firefox-selaimilla.
	- Abitti-koetilapalvelimessa on oletuksena käytössä {{ book.abitti.browser }}-selain, joka on käytännössä Firefox muutamia eroavaisuuksia lukuunottamatta.
	- Tiedossa on, että Internet Explorer -selaimella hallintapaneeli ei välttämättä toimi oikein. Tämä ei ole ongelma *{{ book.abitti.nicename }}*ssa, mutta *{{ book.netti.nicename | lower }}*ssa kylläkin.
- Jotta hallintapaneeliin meneminen onnistuu 17.8.2015 jälkeen päivitetyllä Abitti-palvelintikulla (Abitti-palvelintikun v37 tai uudempi), on Nettiniilon ohjelmistoversion oltava vähintään v1.0.0!* Mikäli näin ei ole, päivitä Nettiniilo ensin <em>{{ book.netti.nicename | lower }}</em>ssa!
- Halutessasi kirjautua hallintapaneeliin, älä kirjoita osoitetta <{{ book.abitti.urls.admin }}> selaimen mahdolliseen hakukenttään ruudun pystysuunnassa keskelle vaan selaimen yläreunassa olevaan osoitekenttään. Paina tämä jälkeen `Enter`.


## WLAN-verkon nimi ja suojausavain

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

<div class="video-container-4by3" style="position:relative; padding-bottom:71.2%; padding-top:30px; height:0; overflow:hidden;">
<iframe style="position:absolute; top:0; left:0; width:100%; height:100%;" width="420" height="315" src="https://www.youtube.com/embed/At4qJw_bkws" frameborder="0" allowfullscreen></iframe>
</div>

<!--![WLAN-verkon nimi ja salasana](https://placehold.it/800x400 "WLAN-verkon nimi ja salasana (tulossa)") -->

### Huomioita WLAN-verkon nimen asettamisesta

Opettaja, mikäli vaihdoit WLAN-verkon nimeä edellä ja mikäli opiskelijoilla oli jo siinä vaiheessa koneet käynnistettynä Abitti-opiskelijantikuilta, kestää opiskelijankoneilla yleensä noin 10-20 sekuntia tajuta, että Nettiniilon tarjoaman verkon nimi on muuttunut. Tänä aikana opikelijan WLAN-verkkoon liittymisen valikossa saattaa hetkellisesti näkyä sekä vanha että uusi verkon nimi tai ei kumpaakaan.

## Loppusilaus ja sitten on valmista!

Nyt sinulla on Abitti-verkko valmiina käyttöön. Tee vielä seuraavat toimet niin voitte aloittaa Abitti-järjestelmän käytön opiskelijoiden kanssa:

1. Lataa koepaketti [oma.abitti.fi](https://oma.abitti.fi)-palvelusta muistitikulle eli nk. *siirtotikulle*.
2. Liitä muistitikku Abitti-koetilapalvelimen roolia toimittavaan koneeseen.
3. Valitse koetilapalvelimella käyttöön siirtotikulle tallentamasi koetiedosto ja syötä oma.abitti.fi-palvelusta tiedostoa varten saamasi purkuavain.
4. Nyt pääsette aloittamaan sähköisen kokeen!

![Kuva tai video koepaketin tuonnista käyttöön](https://placehold.it/800x400 "Kuva tai video koepaketin tuonnista käyttöön (tulossa)")