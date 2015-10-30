# Tiedossa olevia Nettiniilon kehityskohtia

Tälle sivulle on listattu tiedossa olevia Nettiniiloon liittyviä kehitys- tai ongelmakohtia. Aiheet on jaoteltu mahdollisesti korjattaviin ja niihin, joita ei aiota tai voida Nettiniilosta riippumattomista syistä korjata.

## Tehtävälistalla olevat

Seuraavat asiat ovat joko tehtävälistalla tai niiden toteuttamisen mahdollisuutta tutkitaan. Listausjärjestys ei välttämättä implikoi prioriteettijärjestystä.

|Opet | Opisk | IT | Moodi | Kuvaus           | Status  |
|:---:|:-----:|:--:|-------|------------------|---------|
| x   | x     |    | Abitti, Netti| Tiedostoja opiskelijoille jaettaessa tiedostonimet eivät saa tällä hetkellä sisältää ääkkösiä eivätkä lainausmerkkejä. Ääkkösten mahdollistaminen on tarpeen. | korjataan |
| x   | x     |    | Netti | Opiskelijoiden on liityttävä Nettiniilon tarjoamaan langattomaan verkkoon noin yksi opiskelija per 1-2 sekuntia. | parannetaan |
| x   | x     |    | Netti | Jos *{{ book.netti.nicename }}*ssa ei ole yhteyttä Internetiin, ei uudelleenohjaus rekisteröintisivulle toimi vaan käyttäjä joutuu menemään <{{ book.netti.urls.landing }}>. | korjataan |
| x   | x     |    | Netti | Nettiyhteysrajauksen ollessa käytössä iPadeilla (ja ehkä myös iPhoneilla) Safari-selain ei toimi oikein. Käytä Chrome-selainta. Ratkaisumahdollisuutta tutkitaan. | tutkitaan |
|     |       | x  | Netti | Staattisen IP-osoitteen asettaminen Nettiniilon WAN-puolelle. | todo |
|     |       | x  | Netti | Nettiniilon tarjoaman WLAN-verkon käyttämän kanavan manuaalivalinta | todo |
|     |       | x  | Netti | WAN-puolelle mahdollisuus asettaa http-proxy-palvelin. | tutkitaan |
| x   | x     | x  | Abitti| Nettiyhteys *{{ book.abitti.nicename }}*ssa Nettiniilon tarjoaman proxy-palvelimen kautta. | tutkitaan |


## Ei korjata

Tässä tiedossa olevia ongelmakohtia, joita ei ole aietta korjata tai joiden korjaaminen on yksinkertaisesti Nettiniilon kehityksen ulottumattomissa esimerkiksi johtuen laitevalmistajien päätöksistä ja/tai teollisuusstandardeista:

|Opet | Opisk | IT | Moodi | Kuvaus           |
|:---:|:-----:|:--:|-------|------------------|
| x   |       |    | Netti | Hallintapaneeli ei toimi Internet Explorer -selaimen versiota 11 vanhemmilla versioilla. |
| x   |       | x  | Abitti, Netti | Mikäli opettajalla on kone kytkettynä ethernet-kaapelilla Nettiniiloon kun Nettiniilon toimintamoodia vaihdetaan, täytyy ethernet-kaapeli irroittaa 10-15 sekunniksi (päätelaitteen käyttöjärjestelmän on tajuttava IP-osoiteavaruuden muutos ja tämä tapahtuu parhaiten pakottamalla yhteys hetkeksi poikki) |
| x   |       | x  | Netti | Mikäli opettaja liittyy laitteeseen sekä ethernet-kaapelilla että langattomasti, ei opettaja välttämättä pääse kirjautumaan Nettiniilon hallintapaneeliin tai kykene muutenkaan hyödyntämään laitetta. Opettajan päätelaitteen käyttöjärjestelmä ei välttämättä ymmärrä useaa yhtäaikaista uplink-yhteyttä. |
| x   |       |    | Netti | Osoiterajaukset voi tehdä vain domain-tasolla, ts. kun esimerkiksi osoite `http://joku.domain.fi` on sallittuna niin kaikki muotoa `http://joku.domain.fi/....` olevat osoitteet ovat sallittuja.<sup>1</sup> |
| x   | x     |    | Netti | Jos nettiyhteyden rajaus on päällä ja opiskelija yrittää mennä verkkopalveluun, joka ei ole sallittujen joukossa ja ko. verkkopalvelu käyttää HTTPS-protokollaa, ei käyttäjälle näytetä Nettiniilon pääsynestoilmoitusta.<sup>2</sup> |

### Huomioita puutteisiin, joita ei korjata

1. Salaamattomissa yhteyksissä (`http://`) alasivukohtainen rajaus olisi teknisesti mahdollista. Tulevaisuudessa kuitenkin verkkopalvelut tulevat kuitenkin (osaltaan HTTP/2-protokollan yleistymisen myötä) enenevässä määrin käyttämään salattuja yhteyksiä (`https://`). Salatuissa yhteyksissä alasivukohtaisen rajauksen toteuttaminen vaatisi HTTPS-sertifikaatin terminoinnin, joka on eettisesti kyseenalaista ja ilman sertifikaattivaroituksen näyttämistä tai *https to http downgrade* -toimenpidettä teknisesti mahdotonta ilman järjestelmätason oikeuksia kaikkiin verkkoa käyttäviin päätelaitteisiin. Tästä syystä Nettiniilon osoiterajausta ei voi tehdä yksittäisen alasivun tasolla nyt eikä tulevaisuudessa.

2. Nettiniilon tarjoaman virheilmoituksen näyttäminen edellyttäisi HTTPS-sertifikaattivaroituksen näyttämistä käyttäjälle kuten edellä. Yksi mahdollisuus olisi näyttää käyttäjälle sertifikaattivaroitus, mutta vastaavasssa tilanteessa esimerkiksi lentokenttien langattomat verkot eivät näytä varoitusta vaan yksinkertaisesti katkaisevat yhteysyrityksen. Nettiniilon suhteen on päätetty toimia samoin.