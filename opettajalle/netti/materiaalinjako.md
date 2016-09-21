# Nettiniilon materiaalinjako {{ book.netti.nicename }}ssa

<!-- toc -->

Nettiniilon ollessa {{ book.netti.nicename }}ssa on opiskelijoille mahdollista jakaa tiedostoja Nettiniilon USB-porttiin liitetyltä muistitikulta; jaettavaa materiaalia voi käyttää esimerkiksi täydentämään julkisessa Internetissä tai Internetin kautta käytettävässä oppimisympäristössä olevaa aineistoa.

## Näin jaat tiedostoja opiskelijoille

Nettiniilon avulla oheisaineistojen jakaminen Abitti-kokeeseen on suoraviivaista:

1. Kopioi jaettavaksi halutut tiedostot tavalliselle muistitikulle Windows- tai Mac-koneeltasi.
	- Voit käyttää parhaaksi katsomaasi / tottumustesi mukaista tapaa tiedostojen kopiointiin
	- Kopiointitapoja ovat esimerkiksi *raahaa ja pudota* ja *kopioi ja liitä* -toiminnot
2. Irrota muistitikku em. tietokoneesta.
3. Varmista, että Nettiniilo on *{{ book.netti.nicename }}ssa*.
4. Liitä oheisaineistot sisältävä muistitikku Nettiniilon USB-porttiin.
5. Varmista, että opiskelijat ovat käynnistäneet koneensa koneen omaan käyttöjärjestelmään (esim. Windows / Apple OS X).
6. Kehota opiskelijoita...
	1. avaamaan uusi selainikkuna (`Ctrl+N`) tai uusi selainvälilehti (`Ctrl+T`),
	2. kirjoittamaan em. ikkunan/välilehden osoiteriville **{{ book.netti.urls.landing }}** ja painamaan `Enter`,
	3. syöttämään tarvittaessa etu- ja sukunimensä ja
	4. em. nimirekisteröitymisen jälkeen klikkaamaan (osoitteessa {{ book.netti.urls.landing }}) linkkiä materiaalipankkiin siirtyäkseen.

## Tuetut tiedostotyypit

Oheisaineistoina voidaan käyttää sellaisia tiedostotyyppejä, joiden tarkastelemiseen/käyttämiseen tarvittavat ohjelmistot opiskelijoilla on koneillaan asennetetuna.

Abitti-järjestelmässä kaikilla opiskelijoilla on ennalta tiedetyt ohjelmat ja asetukset käytössään, mutta {{ book.netti.nicename | lower }}n kanssa käytetään koneiden omia käyttöjärjestelmiä Abitti-järjestelmän sijaan ja tällöin tiedostotyyppien tukeen on kiinnitettävä huomiota:

### Tiedostotyypit, joiden pitäisi toimia suoraan

Olipa käyttäjällä Windows- tai Mac-kone, mikäli hänellä on Chrome- tai Firefox-selain asennettuna niin seuraavien tiedostomuotojen pitäisi toimia suoraan selaimessa ja/tai käyttöjärjestelmän mukana tulevilla ohjelmilla:

- Tavalliset tekstitiedostot (.txt)
- RTF-muotoiset tekstidokumentit (.rtf)
- PDF-tiedostot (.pdf)
- Kuvatiedostot (.png, .jpg, .gif, .svg)
- Äänitiedostot (.mp3, .wav, .ogg)
- Videotiedostot (.mp4, .webm, .ogv)

### Tiedostotyypit, jotka vaativat lisäasennuksia

Muut kuin edellä luetellut tiedostotyypit vaativat, että käyttäjän koneella on asennettuna tiedoston avaamiseen vaadittu sovellus. Tässä muutamia yleisimpiä esimerkkejä:

- *Microsoft Office ja LibreOffice -tiedostot*
	- LibreOffice on ilmainen ohjelma, joka on ladattavissa osoitteesta [www.libreoffice.org](http://www.libreoffice.org)
	- LibreOffice osaa melko hyvin avata ja luoda myös Microsoft Office -tiedostoja
		- Word-tiedostot (.docx ja .doc)
		- Excel-tiedostot (.xlsx ja .xls)
		- Powerpoint-tiedostot (.pptx ja .ppt)
	- Ilmaisuutensa tähden opiskelijoita voi velvoittaa asentamaan LibreOffice-ohjelmiston.
- *GeoGebra-tiedostot* (.ggb)
	- Opetuksessa ja opiskelussa ilmainen ohjelma, [www.geogebra.org](http://www.geogebra.org)
	- Voi velvoittaa opiskelijoita asentamaan

<!--

## Tiedostojen palautus

Nettiniilon ohjelmistopäivityksen version 1.1 myötä opiskelijat voivat myös palauttaa tiedostoja opettajalle menemällä Abitti-järjestelmäään käynnistetyllä selaimellaan tiedostojenpalautuksen osoitteeseen: <{{ book.abitti.urls.upload }}>

Näin ollen Abitti-kokeissa on mahdollista toteuttaa laajempia kysymystyyppejä kun vastaukset eivät ole rajoitettuja Abitti-järjestelmän tarjoamiin pelkkiin tekstivastauksiin.

### Tiedostojenpalautukseen ei pääsyä koetilapalvelimelta

Huomaa, että opettajan koetilapalvelimelta ei ole koetilapalvelimen palomuuriasetuksista johtuen pääsyä tiedostojenpalautuksen mukaiseen osoitteeseen (<{{ book.abitti.urls.upload }}>) vaikka opiskelijoiden Abitti-järjestelmään käynnistetyiltä koneilta kyseiseen osoitteseen onkin pääsy.

-->