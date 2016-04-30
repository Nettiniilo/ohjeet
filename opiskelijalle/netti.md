# Nettiniilo opiskelijalle: *{{ book.netti.nicename | lower }}*

Tämä osio käsittelee asioita, jotka opiskelijan on hyvä tietää käyttäessään Nettiniiloa *{{ book.netti.nicename | lower }}*ssa. Koska opiskelijat eivät varmaankaan oma-aloitteisesti lue näitä ohjeita, on opettajan hyvä lukea nämä ohjeet ja ohjeistaa opiskelijoitaan niiden mukaisesti.

## Nettiniilon langattomaan verkkoon liittyminen

Ideana on liittyä Nettiniilo-laitteen tarjoamaan langattomaan verkkoon kun opettaja niin kehottaa. Opettaja kertoo liityttävän langattoman verkon nimen ja salasanan; verkon nimi saattaa olla esimerkiksi *NettiniiloX* (missä X on joku numero). Alla tarkempia käyttöjärjestelmäkohtaisia liittymisohjeita:

### Verkkoon liittyminen Windows 7 -koneella

1. Etsi oikealta alanurkasta ilmaisinalueelta langattoman verkon kuvake (vähän kuin "portaikko") ![Tarjolla olevien langattomien verkkojen tarkastelu](/images/nettimoodi_wlan-liittyminen_win7-01.png)
2. Klikkaa em. kuvaketta hiiren ykköspainikkeella (yleensä vasen painike)
3. Klikkaa opettajasi mainitseman verkon nimeä, esim. *NettiniiloX*
4. Poista valinta kohdasta *Yhdistä automaattisesti* ja klikkaa *Yhdistä* ![Nettiniilon tarjoamaan langattomaan verkkoon liittyminen](/images/nettimoodi_wlan-liittyminen_win7-02.png)


### Verkkoon liittyminen Windows 8 -koneella

Tulossa...

### Verkkoon liittyminen Windows 10 -koneella

Tulossa...

### Verkkoon liittyminen Apple-kannettavilla

Tulossa...

### Miksi *Yhdistä automaattisesti* -asetusta ei valita?

*Yhdistä automaattisesti* -valinnan poistaminen tehdään seuraavasta syystä: mikäli ko. valinta jätettäisiin voimaan ja Nettiniilon tarjoaman langattoman verkon salasana myöhemmin muutetaan, mutta nimi säilyisi ennallaan ja olit aiemmin liittynyt samaan verkkoon, yrittäisi Windows tällöin liittyä muistettuun/tallennettuun langattomaan verkkoon samalla salasanalla kuin aiemmin ja kun vanha salasana ei enää kelpaakaan, toteaa Windows melko epäinformatiivisesti näin:

![Windowsin ilmoitus jos Nettiniilon salasana muutettu, mutta verkon nimi ennallaan](/images/nettimoodi_wlan-liittyminen_win7-salasanavirhe.png "Näin Windows 7 toteaa jos muistetun verkon salasana on muutettu")

## Etu- ja sukunimen syöttäminen

Päästäksesi käyttämään Internet-yhteyttä täytyy sinun rekisteröityä syöttämällä etu- ja sukunimesi. Toimi seuraavalla tavalla:

1. Avaa Internet-selaimesi, esimerkiksi [Chrome](https://www.google.com/chrome/), [Firefox](https://www.mozilla.org/fi/firefox/new/), [Opera](http://www.opera.com/fi) tai [Internet Explorer / Edge](https://www.microsoft.com/fi-fi/windows/microsoft-edge).
2. Mikäli selaimesi ei automaattisesti siirtynyt Nettiniilon rekisteröintikaavakkeeseen, kirjoita selaimesi osoiteriville: *<{{ book.netti.urls.landing }}>* ja paina `Enter`
3. Syötä etu- ja sukunimesi rekisteröintikaavakkeeseen.
4. Paina *Rekisteröidy* -nappia.

Kun olet nyt rekisteröitynyt Nettiniiloon nimelläsi, pääset käyttämään Internet-yhteyttä Nettiniilon kautta.

<!--
* Jos koulun koneilla käytössä proxy- eli välityspalvelin, on se otettava koneelta pois päältä, jotta Nettiniilon *{{ book.netti.nicename | lower }}*a voi käyttää
* Ohjeista rekisteröityminen aina verkkoon kirjautumisen jälkeen 192.168.1.1
-->