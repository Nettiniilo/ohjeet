# Tietoa Nettiniilon ohjelmistoversiosta

## Versionumerointi

### Versiosta 1.0.0 alkaen

Versiosta 1.0.0 alkaen Nettiniilon ohjelmiston versionumerointi noudattaa [Semantic Versioning](http://semver.org/) -periaatteita. Versionumero on siis muotoa *MAJOR*.*MINOR*.*PATCH*, missä:

- *MAJOR*-numeron muuttuessa päivitys aiheuttaa aiemman käytön näkökulmasta epäyhteensopivia muutoksia, ts. käyttäjä joutuu opettelemaan tekemään ainakin yhden ennestään tutun asian uudella tavalla. *MAJOR*-version muutos voi myös tuoda Nettiniiloon uusia ominaisuuksia tai sisältää *PATCH*-tyyppisiä toiminnallisuus- tai tietoturvakorjauksia.
- *MINOR*-numeron muuttuessa päivitys tuo mukaan uusia toiminnallisuuksia muttei oleellisesti muuta ennestään tuttuja ominaisuuksia käyttäjän näkökulmasta. *MINOR*-numeron muutos saattaa sisältää myös *PATCH*-tyyppisiä muutoksia.
- *PATCH*-numeron muuttuessa päivitys korjaa mahdollisia ohjelmistovirheitä tai parantaa laitteen tietoturvaa tms. muttei tuo uusia ominaisuuksia eikä oleellisesti muuta ennestään käytössä olleiden ominaisuuksien käyttötapaa.


#### Versiopäivitysten kiireellisyys

Tässä pähkinänkuoressa tieto siitä missä tilanteessa tietyn ohjelmistopäivityksen asentaminen Nettiniiloon on tarpeellista:

- ***MAJOR*-version muutos:** päivittämistarve ei kiireellinen ellei toisin mainita.
- ***MINOR*-version muutos:** päivittämistarve ei kiireellinen ellei toisin mainita.
- ***PATCH*-version muutos:** päivittäminen suositeltavaa mahdollisimman pian ellei toisin mainita.


### Beta-versiot ennen versiota 1.0.0

Ennen versiota 1.0.0 Nettiniilon ohjelmistoversiot numeroitiin päivämäärän mukaan, aluksi muodossa VV.KK.PP ja sitten VVVV-KK-PP.


## Versiohistoria

Tässä on listattuna Nettiniilon ohjelmistoversiot niin, että vanhin versio on alimpana kunkin version yhteydessä on listattu ne ominaisuudet, jotka ovat käyttäjän näkökulmasta muuttuneet jollain tavalla.

<dl>
<dt>v1.0.1 (5.11.2015)</dt>
<dd>
	<ul>
		<li><em>HUOM! Tätä päivitystä ei tarvitse asentaa mikäli</em>
			<ul>
				<li>käytätte Nettiniiloa vain Abitti-moodissa tai</li>
				<li>ette ole huomanneet nettimoodin osoiterajauksissa ongelmaa, jossa hallintapaneelin mukaan domain-rajauksia ei ole päällä, mutta käytännössä vaikuttaisi siltä, että osoiterajauksia on päällä.</li>
			</ul>
		</li>
		<li>Nettimoodissa verkkoon nimellä rekisteröidyttäessä rekisteröintinapin teksti muutettu muodosta <em>Käytä nettiä</em> muotoon <em>Rekisteröidy</em>.</li>
		<li>Varmistus ettei nettimoodin osoiterajaus jää päälle Nettiniilon uudelleenkäynnistyksen yhteydessä.</li>
		<li>Nettiniilon hallintapaneelin yksiriviset tietokentät näyttävät epäkelvot (esim. liian lyhyet) syötearvot punaisella.</li>
		<li>Pyritään estämään selainta tallettamasta hallintapaneelin HTML-koodia omaan välimuistiinsa. Tällä on merkitystä lähinnä Nettiniilon ohjelmistoa päivitettäessä niin, että vanha versionumero jää pienemmällä todennäköisyydellä näkyviin hallintapaneelin alareunaan päivityksen jälkeen v1.0.1 eteenpäin päivitettäessä.</li>
		<li>Hallintapaneelin etusivun Nettiniilo-logo pienemmäksi.</li>
	</ul>
</dd>
<dt>v1.0.0 (25.8.2015)</dt>
<dd>
	<ul>
		<li>Ilmoita käyttäjälle laitteen ohjelmistoa päivitettäessä mikäli tarjottu päivitystiedosto ei ole tarjoitettu kyseiselle laitealustalle</li>
		<li>Hallintapaneelin salasanan vaihtaminen on nyt mahdollista. Salasana säilyy Nettiniilon ohjelmistopäivityksen yhteydessä tästä versiosta eteenpäin.</li>
		<li>Langattoman verkon asetukset säilyvät Nettiniilon ohjelmistopäivityksen yhteydessä tästä versiosta eteenpäin.</li>
		<li>YTL:n Abitti-palvelimeen tekemien muutoksien johdosta *{{ book.abitti.nicename }}*ssa Nettiniilon hallintapaneeliin on mentävä tästä eteenpäin osoitteen <{{ book.abitti.urls.admin }}> kautta. Nettiniilo tukee hallintapaneeliin menemistä varten sekä vanhaa porttimääritystä (8020) vanhempia v37 aiempia Abitti-tikkuja varten että uutta porttimääritystä (80).</li>
	</ul>
</dd>
<dt>v2015-07-28 beta (28.7.2015)</dt>
<dd>
	<ul>
		<li>Materiaalinjako siirretty *{{ book.netti.nicename }}*ssa portista 80 porttiin 8888</li>
		<li>Käyttäjälle annettavia tietoja/ohjeita parannettu estetyn domainin tapauksessa</li>
	</ul>
</dd>
<dt>v2015-07-23 beta (23.7.2015)</dt>
<dd>
	<ul>
		<li>Huomioi Chromebookien NetBIOS-/host-nimenä käyttämä * hallintapaneelin Status-näkymässä</li>
	</ul>
</dd>
<dt>v2015-05-18 beta (18.5.2015</dt>
<dd>
	<ul>
		<li>Hallintapaneelin Status-näkymässä näytetään nyt erillisessä sarakkeessaan myös verkosta pois käyneet</li>
		<li>Lisätty Status-näkymään tieto, että status-seurantaa tehdään vain silloin kun ko. näkymä on auki</li>
	</ul>
</dd>
<dt>v2015-05-09 beta (9.5.2015)</dt>
<dd>
	<ul>
		<li>Osa USB-tikuista (esim. Maxell) ei toiminut Nettiniilon kanssa; korjattu</li>
		<li>Materiaalinjaon sanamuotoja parannettu kun USB-muistia ei ole kytkettynä</li>
	</ul>
</dd>
<dt>v15.04.14 beta (14.4.2015)</dt>
<dd>
	<ul>
		<li>Materiaalinjaon ohjeistusta parannettu kun USB-muistia ei ole kytkettynä</li>
		<li>Materiaalinjaon auto-refresh USB-tikun Nettiniiloon kytkemisen yhteydessä</li>
		<li>Nettirajauksen suorituskykyä parannettu</li>
	</ul>
</dd>
<dt>v15.04.07 beta (7.4.2015)</dt>
<dd>
	<ul>
		<li>Laitteen versiotieto ja valmistajan yhteystiedot lisätty hallintapaneelin alareunaan</li>
		<li>Hallintapaneelin käyttäjäsyötevalidointia parannettu</li>
		<li>Päivitystoiminnon virhesietoisuutta parannettu</li>
		<li>Käyttäjälle näytettäviä virheilmoituksia selvennetty</li>
	</ul>
</dd>
<dt>v15.03.22 beta (22.3.2015)</dt>
<dd>
	<ul>
		<li>*{{ book.netti.nicename }}*n rekisteröintisivun ulkoasua ja toimintaa parannettu</li>
		<li>Laitteen NetBIOS-/host-nimen ja IP-osoitteen näyttö *{{ book.netti.nicename }}*ssa hallintapaneelin Status-näkymässä kun oppilas ei vielä ole rekisteröitynyt</li>
		<li>Päivitystoiminnon korjaus</li>
		<li>Hallintapaneelissa WLAN- ja nettirajaussyötteiden validointia parannettu</li>
	</ul>
</dd>
<dt>v15.03.20 beta (20.3.2015)</dt>
<dd>Ensimmäinen julkaistu versio</dd>
</dl>