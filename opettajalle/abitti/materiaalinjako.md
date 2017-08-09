# Nettiniilon materiaalinjako {{ book.abitti.nicename }}ssa

<!-- toc -->

Abitti-järjestelmä tarjoaa mahdollisuuden jakaa opiskelijoille liitetiedostoja, mutta Abitin lähestymistapa asiaan <kbd>attachments.zip</kbd> -tiedoston luontineen on käytännön tasolla osoittautunut opettajille haastavaksi.

## Näin jaat tiedostoja opiskelijoille

Nettiniilon avulla oheisaineistojen jakaminen Abitti-kokeeseen on suoraviivaista:

1. Kopioi jaettavaksi halutut tiedostot tavalliselle muistitikulle Windows- tai Mac-koneeltasi.
	- Voit käyttää parhaaksi katsomaasi / tottumustesi mukaista tapaa tiedostojen kopiointiin
	- Kopiointitapoja ovat esimerkiksi *raahaa ja pudota* ja *kopioi ja liitä* -toiminnot
2. Irrota muistitikku em. tietokoneesta.
3. Varmista, että Nettiniilo on *{{ book.abitti.nicename }}ssa*.
4. Liitä oheisaineistot sisältävä muistitikku Nettiniilon USB-porttiin.
5. Varmista, että opiskelijat ovat käynnistäneet koneensa Abitti-opiskelijantikuilta.
6. Kun Abitti-koe on aloitettu, näkyy opiskelijoilla kokeen yläreunassa nappi/linkki ***Nettiniilon materiaalinjako***

***Huomaa***, että voit jakaa Nettiniilon avulla oheisaineistoja myös kaapeliyhteydellä toteutettuun Abitti-verkkoon! [Lisätietoja](../../yllapitajalle/abitti.md#aineistojen-jakaminen-nettiniilon-avulla-abitti-kaapeliverkkoon).

### Mikäli jaetut aineistot eivät näy opiskelijoille

Mikäli nappia/linkkiä Nettiniilon materiaalinjakoon ei näy opiskelijoiden kokeen yhteydessä, toimi näin:

1. Kehota opiskelijoita lataamaan koenäkymä uudestaan (`Ctrl+R` tai `F5`, Apple: `Cmd+R`)
2. Mikäli edellä mainittukaan ei auttanut, kehoita opiskelijoita avaamaan uusi selainikkuna (`Ctrl+N`) tai uusi välilehti (`Ctrl+T`) ja
3. kirjoittamaan em. ikkunan/välilehden osoiteriville **{{ book.abitti.urls.share }}** ja painamaan `Enter`.

### Tietoa linkistä Nettiniilon materiaalinjakoon

Mikäli:

- Abitti-koe on laadittu käyttäen [Tweak-A-bitti](https://bit.ly/abitti-chrome) -selainlaajennusta,
- Nettiniilo on käytössä joko yhteyksien muodostamiseen tai vain materiaalinjakoa varten ja
- Nettiniilon USB-porttiin on liitettynä muistitikku, joka sisältää jaettavaksi haluttuja tiedostoja

niin opiskelijalle näkyy kokeen yhteydessä nappi/linkki Nettiniilon materiaalinjakoon.

### Materiaalinjakolinkin näkymisen toimintaperiaate

- Tweak-A-bitti -selainlaajennus lisää laaditun Abitti-kokeen yhteyteen napinlisäystoiminnon.
- Kun Abitti-koe aloitetaan, em. toiminto tarkistaa onko koeverkossa Nettiniiloa ja jos on, onko Nettiniilon USB-porttiin liitettynä muistitikkua.
	- Jos Nettiniilo ja muistitikku löytyvät, näytetään nappi/linkki Nettiniilon materiaalinjakoon.
- Mikäli Nettiniiloa tai muistitikkua ei löydy
	- opiskelijan kone siirtyy tarkistamaan 10 sekunnin välein onko materiaalinjako otettu käyttöön (Nettiniilo paikalla ja muistitikku liitettynä Nettiniiloon).
	- opiskelijan kone jatkaa em. tarkistamista viiden (5) minuutin ajan. Mikäli tämän ajan sisällä jaettavaa aineistoa ei löytynyt, lopettaa opiskelijan kone yrittämästä löytää aineiston.
	- Em. yritysajan saa aloitettua uudelleen lataamalla koekäyttöliittymän uudestaan kullakin opiskelijankoneella painamalla `Ctrl+R` tai `F5` (Apple: `Cmd+R`).

## Tuetut tiedostotyypit

Oheisaineistoina voidaan käyttää kaikkia Abitti-opiskelijankoneella avattavissa olevia tiedostotyyppejä, joita ovat mm. seuraavat:

- Microsoft Office -tiedostot
	- Word-tiedostot (.docx ja .doc)
	- Excel-tiedostot (.xlsx ja .xls)
	- Powerpoint-tiedostot (.pptx ja .ppt)
- LibreOffice-tiedostot
- Tavalliset tekstitiedostot (.txt)
- PDF-tiedostot (.pdf)
- Kuvatiedostot (muun muassa: .png, .jpg, .gif, .svg, .psd, .xcf)
- GeoGebra-tiedostot (.ggb)
- Äänitiedostot (.mp3, .wav, .ogg)
- Videotiedostot (.mp4, .avi, .mov, .webm, .ogv)
- Texas TI-Nspire -tiedostot (.tns, .tnsp)
- Casio ClassPad -tiedostot (.vcp, .xcp)
- JavaScript-ohjelmia (esim. HTML5-muotoiset [PhET-simulaatiot](https://phet.colorado.edu/fi/simulations/category/html))


## YTL:n toimien vaikutus materiaalinjakoon

Huomaathan, että oheisaineistojen eri tiedostotyyppien avautuvuus suoraan selaimessa ja toisaalta toimivuus ylipäätään Abitti-opiskelijankoneilla on kiinni Ylioppilastutkintolautakunnan Abitti-opiskelijantikuille sisällyttämistä ohjelmista ja niiden asetuksista.

Abitti-käynnistystikkujen versiopäivitysten myötä tuetut tiedostotyypit saattavat muuttua niin, että

- uusia tiedostotyyppejä saattaa tulla tuetuksi ja/tai
- joidenkin aiemmin tiedostotyyppien tuki saattaa poistua.

Tähän on Nettiniilon tasolla mahdoton vaikuttaa.


<!--

## Tiedostojen palautus

Nettiniilon ohjelmistopäivityksen version 1.1 myötä opiskelijat voivat myös palauttaa tiedostoja opettajalle menemällä Abitti-järjestelmäään käynnistetyllä selaimellaan tiedostojenpalautuksen osoitteeseen: <{{ book.abitti.urls.upload }}>

Näin ollen Abitti-kokeissa on mahdollista toteuttaa laajempia kysymystyyppejä kun vastaukset eivät ole rajoitettuja Abitti-järjestelmän tarjoamiin pelkkiin tekstivastauksiin.

### Tiedostojenpalautukseen ei pääsyä koetilapalvelimelta

Huomaa, että opettajan koetilapalvelimelta ei ole koetilapalvelimen palomuuriasetuksista johtuen pääsyä tiedostojenpalautuksen mukaiseen osoitteeseen (<{{ book.abitti.urls.upload }}>) vaikka opiskelijoiden Abitti-järjestelmään käynnistetyiltä koneilta kyseiseen osoitteseen onkin pääsy.

-->