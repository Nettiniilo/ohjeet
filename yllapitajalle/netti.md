# Nettiniilo ylläpitäjälle: *{{ book.netti.nicename | lower }}*

<!-- toc -->

## {{ book.netti.nicename }}n tavoite

Nettiniilon *{{ book.netti.nicename | lower }}* mahdollistaa opettaja- ja oppituntikohtaisen Internet-yhteyden rajaamisen niin, että opettaja voi sallia opiskelijoille pääsyn esimerkiksi vain valitsemaansa sähköiseen oppimisympäristöön tai koepalveluun ja mahdollisesti joihin lähdeainestoksi käyttöön haluamiinsa verkkopalveluihin kuten uutissivustoihin tai vastaaviin.

## {{ book.netti.nicename }}n käytön edellytykset

Jotta Nettiniiloa voidaan hyödyntää {{ book.netti.nicename | lower }}ssa täytyy käytettävissä olla sopiva Internet-yhteys Nettiniilosta eteenpäin. Ideana on, että opiskelijat liittyvät Nettiniilon tarjoamaan langattomaan verkkoon, opettaja voi seurata verkkoon liittyneitä ja siitä poistuneita ja opettaja voi asettaa mihin Internet-domaineihin Nettiniilon tarjoaman langattoman verkon kautta on pääsy.

Internet-yhteys voidaan jakaa Nettiniiloon usealla tavalla; [lisätietoa](./../opettajalle/netti/nettiniilon-hallinta.md#internet-yhteyden-muodostaminen-nettiniilosta).

*Mikäli yhteys halutaan muodostaa liittämällä Nettiniilon *WAN/LAN*-portti (NAT-laitteen WAN-puoli) koulun olemassa olevaan ethernet-yhteyteen, lue alla oleva osio teknisistä tiedoista!*


## Teknistä tietoa moodista

{{ book.netti.nicename }}ssa ollessaan Nettiniilo toimii NAT-reitittimenä, ts. *PoE LAN* -portin ja jakamansa langattoman verkon suuntaan Nettiniilo toimii tällöin DHCP- ja DNS-palvelimina.

***VAROITUS:*** Koska Nettiniilo toimii {{ book.netti.nicename | lower }}ssa *PoE LAN* -portin suuntaan DHCP- ja DNS-palvelimina, ***on erittäin tärkeää ettei {{ book.netti.nicename | lower }}ssa olevan Nettiniilon *PoE LAN* -porttia kytketä koulun olemassaolevana ethernet-verkkoon!*** Tästä varoitetaan Nettiniilon mukana tulevien ohjeiden ensimmäisessä kappaleessa ja lisäksi käsketään kysymään lupa rehtorilta mikäli Nettiniilon *WAN/LAN*-portti haluttaisiin liittää koulun ethernet-verkkoon rajatun Internet-yhteyden jakamiseksi opiskelijoille. Huomaathan, että uplink-yhteys Nettiniilosta Internetin suuntaan voidaan muodostaa *WAN/LAN*-portista koulun seinään kytketyn ethernet-kaapelin lisäksi [muillakin tavoilla](./../opettajalle/netti/nettiniilon-hallinta.md#internet-yhteyden-muodostaminen-nettiniilosta).

Nettiniilo tarjoaa HTTP-palvelinohjelmiston kautta nimirekisteröintiin käytettävän Captive Portal -toteutuksen ({{ book.netti.urls.landing }}), johon käyttäjä ohjataan yrittäessään käyttää nettiä Nettiniilon kautta (uudelleenohjaus tehdään teknisistä syistä vain mikäli käyttäjä yritti mennä HTTP-osoitteeseen, ei HTTPS-osoitteille). Ennen nimirekisteröinnin tekemistä kaikki yhteydenottoyrityksen Internetin suuntaan estetään. Mikäli nimirekisteröinti ei avaudu käyttäjälle automaattisesti, tulee hänen mennä osoitteeseen {{ book.netti.urls.landing }} rekisteröityäkseen.

Lisäksi HTTP-palvelinohjelmiston kautta on toteutettuna hallintapaneeli ({{ book.netti.urls.admin }}) ja materiaalinjakopalvelun ({{ book.netti.urls.share }}).


<!--
## Nettiniilon palauttaminen tehdasasetuksiin

Nettiniilo on mahdollista palauttaa viimeisimmän ohjelmistopäivityksen mukaiseen tehdasasetustilaan. Tehdasasetusten palauttaminen asettaa kaikki salasanat ja muut asetukset oletusarvoihinsa.

Tehdasasetusten palauttaminen tapahtuu seuraavasti:

1. Käynnistä Nettiniilo ja odota, että WLAN-valo syttyy.
2. Pidä Nettiniilon pohjassa oleva `Reset`-näppäin pohjassa vähintään 8 sekunnin ajan.
3. Vapauta Reset-näppäin.
4. Odota, että Nettiniilo käynnistyy nyt uudestaan. Tehdasasetukset ovat palautuneet.


* Jos koulun koneilla käytössä proxy- eli välityspalvelin, on se otettava koneelta pois päältä, jotta Nettiniilon *{{ book.netti.nicename | lower }}*a voi käyttää

* Käytettävä IP-osoiteavaruus
* WiFi Analyzer
* Monta Nettiniiloa samassa tilassa
* Monta eri koetta *{{ book.abitti.nicename }}*ssa yhdessä Nettiniilolla (kyllä, kunhan Abitti-palvelin tukee)
-->