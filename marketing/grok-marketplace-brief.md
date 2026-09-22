# Ohje Grok-botille: Clubbook myyntiin App Storeen

Tämä on toimintakäsky. Noudata sitä sellaisenaan. Älä avaa alla lukittuja päätöksiä uudelleen, ellet löydä Applelta tuoreempaa virallista sivua, joka kumoaa ne.

Tuote on Clubbook (repositorio `clubbook`, aiemmin Mailakirja): yhden pelaajan etäisyyskirja. Carry ja total mailoittain, sää- ja korkeuskorjaus, kalibrointi yhdellä lyönnillä, Trackman-tuonti, nimettävät lyönnit, metrit tai jaardit. Data pysyy laitteessa. Tiliä ei ole.

## Lukitut päätökset

1. Myyntikanava on Apple App Store, ei sovelluksen sisäinen mainosverkosto.
2. Hinta on kertamaksu. Suomessa ja muussa euroalueessa **€1,99**. Yhdysvalloissa **$1,99**. Älä ehdota €1,90. Se ei ole App Storen hintapiste. €1,99 on (vastaa vanhaa Tier 2:ta, tarkistettu Applen hintamatriisista 2026).
3. Ei tilausta. Työkalua käytetään vuosia, ja kertamaksu on siihen sopiva.
4. Ei mainos-SDK:ta, ei banneria, ei palkintovideota. Kentällä mainos on huonompi kuin €1,99.
5. Apple Search Ads on eri asia kuin sovelluksen sisäiset mainokset. Sitä saa suunnitella, mutta kampanjaa ei käynnistetä ennen kuin versio on App Storessa tilassa Approved.
6. Älä lupaa viikoittaisia päivityksiä. Sovellus ei putoa kaupasta, vaikka sitä ei päivitettäisi joka kuukausi.

## Miksi €1,99 eikä mainoksia

Niche on pieni: golfari, joka haluaa mailamitat mukaan kierrokselle. Mainosverkosto tarvitsee paljon avauksia, seurantaluvan ja SDK:n. Ne heikentävät sovellusta, jonka ainoa työ on näyttää luku nopeasti. €1,99 on kynnys, jonka kohderyhmä maksaa kerran.

Apple veloittaa Small Business Programissa 15 %, jos edellisen kalenterivuoden tuotot ovat enintään 1 miljoona USD. €1,99:stä kehittäjälle jää karkeasti €1,69 ennen veroja. Ilman ohjelmaa komissio on korkeampi. Ilmoittaudu ohjelmaan ennen julkaisua.

Kohdennettu mainospaikka tulee mukaan vasta toisessa vaiheessa: Apple Search Ads, exact match, ei display-verkostoa sovelluksen sisällä.

## Mitä kauppaan pääsy vaatii

Tuota puuttuvat tekstit ja merkitse, mikä on jo olemassa. Älä väitä, että HTML-tiedoston voi ladata App Storeen.

1. Apple Developer Program, 99 USD vuodessa. Account Holder hoitaa sopimukset.
2. Paid Applications -sopimus sekä pankki- ja verotiedot App Store Connectissa.
3. Small Business Program -ilmoittautuminen.
4. Julkinen yksityisyyskäytäntö. Sovellus ei luo tiliä eikä lähetä analytiikkaa. Kirjoita käytäntö sen mukaan, englanniksi ja suomeksi. URL tarvitaan ennen lähetystä.
5. Tukisähköposti ja tukisivun URL.
6. Ikäluokitus 4+.
7. Kuvakaappaukset oikeista näkymistä: 6,7 tuuman iPhone ja 6,5 tuuman iPhone. Ei keksittyjä lukuja, ei tekstiä kuvan päällä, joka ei näy itse sovelluksessa.
8. Kuvake 1024×1024, ei läpinäkyvyyttä.
9. App Store -tekstit: nimi, alaotsikko (enintään 30 merkkiä), avainsanat (enintään 100 merkkiä, nimeä ei toisteta), kuvaus, promootioteksti, ensimmäisen version What's New.
10. Paketointi. Nykyinen sovellus on yksi `index.html`. Kauppaan se kääritään Capacitor-kuoreen, joka toimii offline ja ilman kirjautumista. Ostos on sovelluksen hinta, ei linkki verkkokauppaan. Pelkkä Safari-kirjanmerkki ei läpäise review'ta.
11. Review-muistiinpanot: ei tunnuksia, esimerkkibägi on valmiina.
12. Export compliance: vain tavallinen HTTPS, ei omaa salausta.

## Päivitykset

Jatkuvaa päivitystä ei vaadita, jotta listaus pysyy voimassa. Päivitys tehdään, kun toiminto tai korjaus julkaistaan, ja kun Apple nostaa lähetettävän binaarin minimi-SDK:n. Se tapahtuu tyypillisesti uuden Xcoden myötä keväisin. Vanha hyväksytty versio jää kauppaan. Uutta lähetystä ei hyväksytä vanhalla SDK:lla. Yksi ylläpitokäännös vuodessa riittää, ellei tule vikaa.

## Putki tässä järjestyksessä

### 1. Viesti

Yksi lause: "Your bag, adjusted for today."

Kolme todistetta, ei enempää: kalibrointi yhdellä lyönnillä, Trackman-tuonti, nimettävät lyönnit ja jaardit.

Kiellettyjä sanoja markkinoinnissa: AI, unlock your potential, revolutionary, game-changer, typewriter.

### 2. Kauppatekstit

Kirjoita `marketing/store-listing.md`. Englanti on ensisijainen (US, UK, IE, AU, CA). Suomi on toinen storefront. Älä täytä avainsanakenttää sanoilla, jotka ovat jo nimessä tai alaotsikossa.

### 3. Kuvakaappauskäsikirjoitus

Kuusi ruutua, tässä järjestyksessä. Jokaiseen otsikko, enintään neljä sanaa, ja mitä kuvassa pitää näkyä:

1. Bägi ja päivän prosentti.
2. Mikä maila lipulle.
3. Kalibrointi yhdellä lyönnillä.
4. Asetukset: jaardit ja nimetty lyönti, esimerkiksi Knockdown.
5. Trackman-tuonti ja esikatselu, jossa `7 Iron` yhdistyy `7 Iron`iin.
6. Lukittu wedge, joka ei seuraa päivän kuntokerrointa.

### 4. Haku ja Apple Search Ads

Kirjaa 20 hakusanaa prioriteetilla. Rakenna kampanja, mutta älä käynnistä sitä:

- Budjettiehdotus 10–20 € päivässä kahden viikon kokeiluun, vasta kun listaus on Approved.
- Exact match: brändi Clubbook ja viisi termiä (yardage book, golf club distances, trackman yardages, club gapping, golf bag distances).
- Ei broad matchia ensimmäisellä viikolla.
- Hakusanamainos, ei sovelluksen sisäistä paikkaa.

### 5. Julkaisujärjestys

1. Capacitor-kuori ja TestFlight kymmenelle golfarille.
2. Korjaukset, sitten Submit.
3. Kun tila on Approved: julkaise. Pyydä arviota vasta, kun pelaaja on käyttänyt bägiä kierroksella. Kymmenen oikeaa arviota riittää alkuun.
4. Vasta sitten Apple Search Ads, jos orgaaninen haku ei kata yardage book- ja club gapping -hakuja.

## Valmis toimitus

Yksi tiedosto: `marketing/store-listing.md`. Älä muuta sovelluksen koodia tätä ohjetta suorittaessasi. Älä avaa kehittäjätiliä äläkä lähetä binaaria, ellei ihmisellä ole Apple Developer -jäsenyys ja hän pyytää sitä erikseen.
