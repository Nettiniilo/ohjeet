# Laitteiden käynnistäminen (*{{ book.abitti.nicename }}*)

Jotta Abitti-järjestelmää voidaan käyttää, täytyy käynnistää Abitti-palvelin sekä opiskelijoiden koneet Abitti-käynnistysmuistitikuilta. Lisäksi täytyy käynnistää Nettiniilo ja varmistaa että se on *{{ book.abitti.nicename }}*ssa / asettaa Nettiniilo *{{ book.abitti.nicename }}*in.

Näissä ohjeissa ei käsitellä opiskelijoiden koneiden käynnistämistä Abitti-järjestelmään.

## Nettiniilon käynnistäminen

Ottaaksesi Nettiniilon käyttöön Abitti-järjestelmän kanssa käytettäväksi, toimi seuraavasti:

1. Irrota Nettiniilosta kaikki johdot.
2. Kytke pyöreäpäinen virtajohto Nettiniiloon.
3. Kytke virtajohdon toinen pää seinän virtaliittimeen.
4. Odota, että Nettiniilo käynnistyy.
	- Laite on valmis käytettäväksi kun laitteen etukannessa oleva WLAN-valo syttyy.
	- **HUOM!** Ennen 25.8.2015 toimitettujen Nettiniilojen mukana tulleissa ohjeissa kehotetaan odottamaan WPS-valon vilkkumisen päättymistä. Noudata kuitenkin yllä annettua ohjetta.
5. Varmista, että Nettiniilo on *{{ book.abitti.nicename }}*ssa:
	- Mikäli laitteen päällä oleva WPS-valo palaa, laite on jo *{{ book.abitti.nicename }}*ssa.
	- Mikäli laitteen päällä oleva WPS-valo ei pala:
		- paina WPS-nappia kerran kevyesti (kuulet pienen napsahduksen) ja odota
		- parin sekunnin sisällä WPS-napin painamisesta nappi alkaa vilkkua
		- odota noin 10 sekuntia kunnes napin vilkkuminen päättyy
		- kun WPS-valo jää palamaan, on laite *{{ book.abitti.nicename }}*ssa
6. Jatka ohjeiden seuraavaan vaiheeseen.

![Kuva tai video Nettiniilon käynnistämisestä](http://placehold.it/600x300 "Kuva tai video Nettiniilon käynnistämisestä (tulossa)")


## Koetilapalvelimen käynnistäminen

Abitti-järjestelmän käyttämistä varten tarvitset Abitti-koetilapalvelimen.

1. Mikäli käytät koetilapalvelimena konetta, jossa ei ole ethernet-porttia ja joudut näin ollen käyttämään USB-ethernet-sovitinta (esim. Applen Macbook Air -kannettavat), varmista että USB-ethernet-sovitin on kytkettynä koneeseen ennen seuraavaan vaiheeseen siirtymistä.
2. Käynnistä opettajan koneesi Abitti-koetilapalvelimeksi Abitti-koetilapalvelinmuistitikulta.
3. Jatka ohjeiden seuraavaan vaiheeseen.

## Yhteys Nettiniilon ja koetilapalvelimen välille

Jotta opiskelijoiden Abitti-muistitikuilta käynnistetyt koneet voivat kommunikoida Abitti-koetilapalvelimen kanssa, on niiden välille muodostettava tietoliikenneyhteydet. Nettiniilon avulla tarvittavien tietoliikenneyhteyksien luominen on vaivatonta.

1. Varmista, että olet käynnistänyt Nettiniilon ja että se on *{{ book.abitti.nicename }}*ssa.
4. Kun koetilapalvelin on käynnistynyt, kytke ethernet-johto koetilapalvelimesta Nettiniilon PoE LAN -porttiin.

### Verkkokaavio

![Nettiniilo Abitti-moodissa](/files/images/nettiniilon-kytkenta-abitti-moodissa.png "Nettiniilon kytkentä Abitti-järjestelmää käytettäessä.")