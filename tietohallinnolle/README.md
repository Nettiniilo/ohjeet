# Nettiniilo tietohallinnolle: yleistä

<!-- toc -->

Tämä osio sisältää ensisijaisesti teknisemmin orientoituneille henkilöille kuten koulun IT-vastaaville ja tietohallintohenkilöstölle suunnattua tietoa ja ohjeita.

## Nettiniilon tavoitteet

Nettiniilo on tarkoitettu opettajien ja opiskelijoiden arjen apuvälineeksi. Nettiniilon tavoitteena on:

1. sulavoittaa oppilaitoksen arkea YTL:n Abitti-järjestelmää esimerkiksi kurssikokeissa hyödynnettäessä
2. tarjota mahdollisuus Internet-yhteyden rajaamiseen oppitunti- ja opettajakohtaisesti.

Perinteiset koulu- tai kuntatasoiset tietoliikenneratkaisut eivät usein ole riittävän joustavia edellä mainittujen käyttötapausten näkökulmasta:

1. Ensimmäisen em. kohdan erityisvaatimuksena on IP-osoiteavaruudessa 10.10.x.y toimiva tietoliikenneverkko, jossa YTL:n Abitti-järjestelmän koetilapalvelimella täytyy olla mahdollisuus toimia authoritative-DHCP -palvelimena.
2. Jälkimmäinen tapaus eli Internet-yhteyden oppitunti-/opettaja-/luokkatilakohtainen rajaaminen ei onnistu tavallisilla tietoverkkoratkaisuilla ilman erillisten hallinnointiohjelmistojen asentamista asiakaskoneille.

## Nettiniilon käyttömoodit

Nettiniilossa on edellä kuvattuihin tavoitteisiin liittyen kaksi toisensa poissulkevaa käyttömoodia. Kun laite on käynnistetty ja käyttövalmis, vaihdetaan moodia painamalla laitteen päällä olevaa nappia; moodinvaihtoprosessin suorittamiseen laitteella kestää noin parikymmentä sekuntia. Moodin vaihtumisen aikana napissa oleva valo vilkkuu.

### Moodien nimet ja käyttökontekstit

Nettiniilon käyttömoodit ovat nimeltään {{ book.abitti.nicename }} ja {{ book.netti.nicename | lower }}. {{ book.abitti.nicename }} on nimensä mukaisesti tarkoitettu käytettäväksi yhdessä YTL:n Abitti-järjestelmän kanssa. {{ book.netti.nicename }}a puolestaan käytetään silloin kun *ei käytetä* Abitti-järjestelmää.

Nettiniilon kautta voidiaan sekä {{ book.abtti.nicename }}ssa että {{ book.netti.nicename | lower }}ssa jakaa opiskelijoille tiedostoja Nettiniiloon kytketyltä USB-massamuistilta. {{ book.netti.nicename }}ssa voidaan lisäksi rajata opiskelijoiden Internet-yhteyttä ja seurata ketkä opiskelijat ovat liittyneet päätelaitteillaan Nettiniilon tarjoamaan langattomaan verkkoon.

### Teknistä tietoa moodeista

#### {{ book.abitti.nicename }}

{{ book.abitti.nicename }}ssa olleessaan Nettiniilo toimii teknisesti kytkimenä ja olettaa, että samassa verkossa joku muu laite hoitaa DHCP-palvelimen tehtävät. Nettiniilon IP-osoite on {{ book.abitti.urls.ip }}.

Täydennystä tulossa...