# Tietoa Nettiniilon ohjelmistoversiosta


<!-- toc -->

## Versiohistoria

Tässä on listattuna Nettiniilon ohjelmistoversiot niin, että vanhin versio on alimpana kunkin version yhteydessä on listattu ne ominaisuudet, jotka ovat käyttäjän näkökulmasta muuttuneet jollain tavalla.

*Ohjeet päivittämiseen sekä tarvittavat firmware-tiedostot löydät [Ohjelmistopäivitys ja resetointi](/yllapitajalle/paivittaminen.html) -sivulta.*

<dl>
<dt><a href="/yllapitajalle/paivittaminen.html">v1.1.1</a> (22.9.2016)</dt>
<dd>
	<ul>
		<li>Parannus Nettiniilon materiaalinjaon ulkoasuun {{ book.abitti.nicename }}a käytettäessä.</li>
	</ul>
</dd>
<dt>v1.1.0 (29.4.2016)</dt>
<dd>
	<ul>
		<li>Sekä {{ book.abitti.nicename }} että {{ book.netti.nicename | lower }}:
			<ul>
				<li>Nettiniilon materiaalinjaon kautta jaettuja ääni- ja videotiedostoja voi nyt kelata.</li>
				<li>Nettiniilon muodostaman WLAN-verkon taajuuden/kanavan manuaalivalinta mahdolliseksi.
					<ul>
						<li>Nettiniilon hallintapaneelissa on nyt mahdollista asettaa WLAN-taajuus käsin.</li>
						<li>Tämä ominaisuus on hyödyllinen esim. silloin jos Nettiniilon verkko ja koulun olemassaoleva WLAN-verkko sattuvat "päällekkäin". Todennäköisimmin ette kuitenkaan tarvitse muuttaa tätä pois automaattiasetuksesta.</li>
					</ul>
				</li>
				<li>WPS-napin painalluksella vaihdetaan Nettiniilon käyttötapaa/-moodia {{ book.abitti.nicename }}n ja {{ book.netti.nicename | lower }}n välillä. Tämä päivitys korjaa virheen, jossa WPS-nappia useammin kuin kerran "sopivin väliajoin" painamalla Nettiniilon pystyi saamaan osittaiseen jumitilaan (ja Nettiniilon joutui <a href="/yllapitajalle/paivittaminen.html#nettiniilon-resetointi-eli-palauttaminen-tehdasasetuksiin">resetoimaan</a> pohjassa olevalla Reset-napilla).</li>
				<li>Nettiniilon materiaalinjaon ulkoasua parannettu.</li>
				<li>Pieniä hallintapaneelin käyttöliittymäparannuksia.</li>
			</ul>
		</li>
		<li>{{ book.netti.nicename }}:
			<ul>
				<li>Parannus {{ book.netti.nicename | lower }}ssa Nettiniilon tarjoamaan WLAN-verkkoon liittymisen jälkeisessä nimirekisteröinnissä.
					<ul>
						<li>Käyttäjät ovat raportoineet, että {{ book.netti.nicename | lower }}ssa nimirekisteröintiin pääsy ja rekisteröitymisnapin painalluksen jälkeinen toiminta ovat tahmanneet.</li>
						<li>Syy ongelmaan on selvitetty ja tämän päivityksen pitäisi korjata ongelman.</li>
					</ul>
				</li>
				<li>Lisätty tuki 4G-mokkuloille (ainakin <a href="https://www.google.com/search?q=huawei+e3372&amp;tbm=isch">Huawei E3372</a>).
					<ul>
						<li>Toimii yksinkertaisesti kytkemällä mokkula Nettiniilon USB-porttiin.</li>
						<li>Aiemmin ollut tuki 3G-mokkuloille on voimassa edelleen; 3G-mokkulaa käytettäessä PIN-koodi ja APN-arvo täytyy asettaa Nettiniilon hallintapaneelissa {{ book.netti.nicename | lower }}ssa.</li>
					</ul>
				</li>
				<li>Nettiyhteyden jako Android-kännykästä USB-johdolla Nettiniiloon.
					<ul>
						<li>Testattu Android 4.4 ja Android 5.1 -kännyköillä.</li>
						<li>Liitä kännykkä USB-johdolla Nettiniilon USB-porttiin ja aseta kännykän asetuksista nettiyhteyden jakaminen USB:n kautta päälle.</li>
						<li>iPhone: ei toimi (eikä tod.näk. tulevaisuudessakaan toimi) johtuen Applen epästandardista "iTunes vaaditaan" -tavasta toteuttaa asia.</li>
						<li>Windows Phone: pari vuotta vanhalla Lumialla netin jako USB:n kautta ei toiminut (tai ainakaan käyttöliittymästä/asetuksista ei löytynyt tarvittavaa valintaa).</li>
					</ul>
				</li>
			</ul>
		</li>
	</ul>
</dd>
<dt>v1.0.1 (5.11.2015)</dt>
<dd>
	<ul>
		<li><em>HUOM! Tätä päivitystä ei tarvitse asentaa mikäli</em>
			<ul>
				<li>käytätte Nettiniiloa vain Abitti-moodissa tai</li>
				<li>ette ole huomanneet {{ book.netti.nicename | lower }}n osoiterajauksissa ongelmaa, jossa hallintapaneelin mukaan domain-rajauksia ei ole päällä, mutta käytännössä vaikuttaisi siltä, että osoiterajauksia on päällä.</li>
			</ul>
		</li>
		<li>{{ book.netti.nicename }}ssa verkkoon nimellä rekisteröidyttäessä rekisteröintinapin teksti muutettu muodosta <em>Käytä nettiä</em> muotoon <em>Rekisteröidy</em>.</li>
		<li>Varmistus ettei {{ book.netti.nicename | lower }}n osoiterajaus jää päälle Nettiniilon uudelleenkäynnistyksen yhteydessä.</li>
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
		<li>Materiaalinjako siirretty *{{ book.netti.nicename | lower }}*ssa portista 80 porttiin 8888</li>
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
		<li>Laitteen NetBIOS-/host-nimen ja IP-osoitteen näyttö *{{ book.netti.nicename | lower }}*ssa hallintapaneelin Status-näkymässä kun oppilas ei vielä ole rekisteröitynyt</li>
		<li>Päivitystoiminnon korjaus</li>
		<li>Hallintapaneelissa WLAN- ja nettirajaussyötteiden validointia parannettu</li>
	</ul>
</dd>
<dt>v15.03.20 beta (20.3.2015)</dt>
<dd>Ensimmäinen julkaistu versio</dd>
</dl>

## Tietoa versionumeroinnista

### Versiosta 1.0.0 alkaen

Versiosta 1.0.0 alkaen Nettiniilon ohjelmiston versionumerointi noudattaa [Semantic Versioning](http://semver.org/) -periaatteita. Versionumero on siis muotoa *MAJOR*.*MINOR*.*PATCH*, missä:

- *MAJOR*-numeron muuttuessa päivitys aiheuttaa aiemman käytön näkökulmasta epäyhteensopivia muutoksia, ts. käyttäjä joutuu opettelemaan tekemään ainakin yhden ennestään tutun asian uudella tavalla. *MAJOR*-version muutos voi myös tuoda Nettiniiloon uusia ominaisuuksia tai sisältää *PATCH*-tyyppisiä toiminnallisuus- tai tietoturvakorjauksia.
- *MINOR*-numeron muuttuessa päivitys tuo mukaan uusia toiminnallisuuksia muttei oleellisesti muuta ennestään tuttuja ominaisuuksia käyttäjän näkökulmasta. *MINOR*-numeron muutos saattaa sisältää myös *PATCH*-tyyppisiä muutoksia.
- *PATCH*-numeron muuttuessa päivitys korjaa mahdollisia ohjelmistovirheitä tai parantaa laitteen tietoturvaa tms. muttei tuo uusia ominaisuuksia eikä oleellisesti muuta ennestään käytössä olleiden ominaisuuksien käyttötapaa.


### Versiopäivitysten kiireellisyys

Tässä pähkinänkuoressa tieto siitä missä tilanteessa tietyn ohjelmistopäivityksen asentaminen Nettiniiloon on tarpeellista:

- ***MAJOR*-version muutos:** päivittämistarve ei kiireellinen ellei toisin mainita.
- ***MINOR*-version muutos:** päivittämistarve ei kiireellinen ellei toisin mainita.
- ***PATCH*-version muutos:** päivittäminen suositeltavaa mahdollisimman pian ellei toisin mainita.


### Beta-versiot ennen versiota 1.0.0

Ennen versiota 1.0.0 Nettiniilon ohjelmistoversiot numeroitiin päivämäärän mukaan, aluksi muodossa VV.KK.PP ja sitten VVVV-KK-PP.