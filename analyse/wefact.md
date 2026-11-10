# WeFact – review-analyse

> Focus: offerte en facturatie. WeFact is **geen vakbedrijf-specifiek pakket**. Het is generieke facturatiesoftware voor zzp en mkb. Reviews van vakbedrijven zijn zeldzaam: er zijn er 3 met een herkenbare branche, waarvan 2 uit 2018. Lees de bevindingen dus als "de lat voor facturatie en offerte bij kleine ondernemers", niet als stem van de vakman.

## Profielschets

- **Wie/wat**: WeFact B.V. (Eersel, sinds 2005). Online facturatie: facturen, offertes, abonnementen/periodieke facturen, inkoopfacturen (scan en herken), betalingsherinneringen, iDEAL/incasso, Peppol en een boekhoudkoppeling. De site meldt "tienduizenden gebruikers" en ">1000 accountantskantoren" die WeFact adviseren (bron: JSON-LD op https://www.wefact.nl/prijzen/, opgehaald 2026-11-10). Meerdere reviewers noemen Visma als (nieuwe) eigenaar. Dat is niet geverifieerd op de site van WeFact.
- **Belangrijke context**: **FactuurSturen.nl/.be is gestopt en de klanten zijn naar WeFact gemigreerd.** Die migratie (najaar 2025 tot zomer 2026) drijft het grootste deel van de negatieve reviews.
- **Prijsindicatie** (https://www.wefact.nl/prijzen/, opgehaald 2026-11-10, excl. btw, bij jaarbetaling; per maand tussen haakjes):
  - Small: € 6,50 p/m (€ 6,95), 4 facturen per maand
  - Start 100: € 16,50 p/m (€ 17,25), 100 facturen per maand
  - Start 100 met **Plus**: € 26,50 p/m (€ 27,25), dus +€ 10. Plus omvat onder meer "Automatisch offertes opvolgen", "Offertes in delen factureren", "Inzicht in geopende e-mails", "Taken en interacties", extra documenten zoals **werkbonnen**, pakbonnen en opdrachtbevestiging, en mailings.
  - Losse modules: boekhoudkoppeling € 5 p/m, bankkoppeling € 5 per rekening per maand, productvoorraad € 15 p/m, extra opslag € 2,50 per GB.
  - Proefperiode: 30 dagen gratis.
- **Kernfuncties voor ons onderzoek**: offertes en facturen met eigen briefpapier, offerte-opvolging (alleen in Plus), relatiedossier, mobiele app (iOS en Android) vooral om te bekijken, af te vinken en bonnetjes te scannen. Er is geen planning of agenda en geen lead-opvang. Werkbonnen bestaan alleen als "extra document" in Plus.

## Databasis

| bron | aantal in CSV | wat opgehaald |
|---|---|---|
| Trustpilot (nl.trustpilot.com/review/wefact.nl) | 73 | Profiel: 266 reviews, TrustScore 4,2; verdeling 1★ 25, 2★ 16, 3★ 15, 4★ 57, 5★ 153; "241 reviews in de afgelopen 12 maanden". Opgehaald zijn **alle 31 reviews van 2–3★**, de 20 nieuwste van 1★, de 20 nieuwste van 4★ (1 lege overgeslagen) en 7 via de actor `automation-lab/trustpilot`. |
| App Store NL (id1057713776) | 15 | 35 reviews opgehaald (2016–2026). Opgenomen zijn de inhoudelijke reviews, met nadruk op 2022+ en op vakbedrijven. |
| Google Play (nl.wefact.app.standard) | 9 | 57 reviews opgehaald (2016–2026). Opgenomen zijn de inhoudelijke, kritische of vakgerelateerde reviews. |
| **Totaal** | **97** | |

- **Verdeling** (script over `data/wefact.csv`): 1 ster 27 · midden 49 · positief 21
- **Periode**: 2016-04 t/m 2026-10. **82 van de 97 rijen zijn van na nov 2024.** De oudere rijen zijn bijna allemaal app-reviews: van de 15 App Store-rijen zijn er 5 recent, van de 9 Google Play-rijen 4.
- **Kwaliteitsnoten**:
  - **Bias door gedwongen migratie**: 34 rijen komen van ex-FactuurSturen-gebruikers (19× 1★, 10× 2★, 5× 3★). Zij vergelijken met hun oude pakket en zijn niet zelf voor WeFact gekozen. De pijnpunten "onboarding/migratie" en "lock-in" zijn daardoor sterk oververtegenwoordigd ten opzichte van een normale WeFact-klant.
  - **Golf eind juli 2026**: veel 3- en 4-sterrenreviews dateren van 28 tot 31 juli 2026. Een reviewer schrijft: "Dat ik wordt uitgenodigd voor deze evaluatie…". Er liep dus kennelijk een reviewverzoek, terwijl Trustpilot zegt dat er "geen recente geschiedenis van het vragen naar reviews" is. Een Belgische reviewer suggereert dat positieve reviews gekocht zijn; dat is niet te verifiëren.
  - **Bewust geselecteerd**: de groep positief is ondervertegenwoordigd, omdat we de focus op middenreviews legden. Gebruik de CSV niet als steekproef voor tevredenheid. Daarvoor is de Trustpilot-verdeling (79% 4–5★) de betere indicatie.
  - **Weinig vakbedrijven**: herkenbare vakbedrijven zijn een vermoedelijk technisch bedrijf (artikelbestanden van groothandels, 2026), een schildersbedrijf (2018) en een dakdekker (2018).
  - **Niet opgehaald**: Capterra (WebSearch toonde 1 review; niet opgehaald). De `automation-lab/trustpilot`-actor leverde maar 7 van de 266 reviews, vooral Engelstalig. Daarom zijn de gefilterde Trustpilot-pagina's direct opgehaald via web-fetch. Ingebouwde WebFetch naar wefact.nl werd door de sandbox geblokkeerd.

## Wat gebruikers goed vinden (de lat)

1. **Eenvoud voor de basis**: snel een factuur of offerte maken, overzicht van open en betaalde facturen (positief:gebruiksgemak 15×).
   - "Facturen en offertes maken gaat snel en de interface is duidelijk." (Trustpilot, 4★, 2026-08-03)
   - "Je ziet snel welke facturen betaald zijn en welke open staan…" (Trustpilot, 4★, 2026-08-17)
2. **Persoonlijke en bereikbare support** (positief:support 7×), al zijn er ook klachten over support.
   - "top telefonische assistentie met echte mensen." (Trustpilot, 4★, 2026-07-29)
   - "De helpdesk was goed bereikbaar bij de overstap…" (Trustpilot, 3★, 2026-07-28)
3. **Koppelingen met boekhouder, bank en Mollie** (positief:koppelingen en positief:boekhoudkoppeling samen 7×).
   - "Goed werkende koppelingen met andere software, makkelijk en snel zelf ingericht." (Trustpilot, 4★, 2026-08-02)
   - "De koppeling met de bank en in mijn geval Snelstart loopt goed." (Trustpilot, 3★, 2026-07-29)
4. **Eigen briefpapier en professionele uitstraling**: "Facturen met eigen briefpapier maken is echt goed geregeld." (Trustpilot, 4★, 2026-07-29)
5. **Vakbedrijven (oud, 2018)**: "wij als middelgroot schildersbedrijf hebben hier weinig over op te merken" (App Store, 4★, 2018-12-04). "ons bedrijf dakdekker.nl te koppelen aan WeFact. Dat ging verrassend eenvoudig" (App Store, 4★, 2018-11-08).

## Top 5 pijnpunten

Frequentie = aantal rijen in de CSV met dat thema (alle groepen samen; tussen haakjes 1★ / midden).

| # | thema | freq. | ernst | toelichting |
|---|---|---|---|---|
| 1 | gebruiksgemak (te veel kliks, beperkte opmaak, zoeken/filteren) | 26 (8/18) | middel | het meest genoemde punt in de middenreviews |
| 2 | onboarding/migratie | 21 (12/9) | hoog, maar tijdelijk | vrijwel volledig door de FactuurSturen-migratie |
| 3 | bugs/snelheid | 21 (7/14) | hoog | traag zoeken, betalingen niet geregistreerd, app-crashes na updates |
| 4 | mobiel | 20 (8/11) | middel–hoog | de app is een afgeslankte kijk-app; scannen en uploaden faalt |
| 5 | prijs (Plus-model, prijsverhoging) | 13 (9/4) | middel | functies verschuiven naar betaalde Plus-laag |

Ook genoemd: support 16× (kritisch), facturatie-logica 14×, lock-in/data-export 10×, rapportage 9×.

**1. Gebruiksgemak**
- "herhalende acties kosten soms onnodig veel tijd/kliks." (Trustpilot, 3★, 2026-07-29)
- "Voor eenvoudige basishandelingen, zoals het wijzigen of laten vervallen van een abonnement, zijn onnodig veel stappen en kliks vereist." (Trustpilot, 2★, 2026-07-28)
- "Met name het opmaakgedeelte voor het aanpassen van de lay-out is veel beperkter…" (Trustpilot, 3★, 2026-07-29)

**2. Onboarding/migratie**
- "Automatische overgang van factuursturen is een ramp! Nul begeleiding op voorhand." (Trustpilot, 3★, 2025-11-06)
- "Ik heb dit gedaan en ben toch al mijn administratie kwijt" (Trustpilot, 2★, 2026-01-21)

**3. Bugs/snelheid**
- "In 2 maanden tijd bij 3 verschillende facturen een betaling niet goed geregistreerd of kwijt geraakt. Het gevolg is een onterechte herinnering naar de klant" (Trustpilot, 2★, 2026-04-07)
- "ik moet 35 seconden wachten voordat er een nummer op mijn scherm komt te staan" (Trustpilot, 2★, 2026-07-29)
- "Enige grote nadeel is dat het systeem om de paar maanden weer een uurtje offline is." (Trustpilot, 4★, 2026-07-30)

**4. Mobiel**
- "Na de laatste update al een week een wit scherm." (App Store, 1★, 2026-10-22)
- "fotos die ik maak met mijn telefoon niet binnen komen… .HEIC formaat" (Trustpilot, 2★, 2026-07-31)
- "Het alleen maar kunnen bekijken is zo’n gemiste kans." (App Store, 4★, 2020-01-21; oud)

**5. Prijs**
- "Het onlangs verschenen 'plus' product heeft ervoor gezorgd dat enkele zaken die voorheen standaard waren, nu ineens extra geld kosten." (Trustpilot, 3★, 2026-08-04)
- "Nu 10 euro extra op maandbedrag van 17 euro" (Trustpilot, 2★, 2026-07-29)

## "Wat net mist" (uit middenreviews)

- **Kleine efficiëntie-wensen die jaren blijven liggen.** Voorbeelden: een optelling bij meerdere geselecteerde facturen, bladeren tussen facturen binnen een relatie, de optie "betaald" standaard aan, zoeken op eigen referentie. Reviewers ervaren dat suggesties "genoteerd" worden en daarna niets gebeurt: "ben ik inmiddels gestopt met het aandragen van suggesties" (3★, 2026-07-29).
- **Offerte-flexibiliteit**: "Als je wat uitgebreider offertes of facturen wil maken is het lastig." (3★, 2026-07-29). Ook ontbreken interne notities en bijlagen per dossier die de klant niet ziet: "Eigen bijlage toevoegen voor eigen admin. (die de klant niet kan zien) is er niet!"
- **Betrouwbaarheid van klantcontact rond de factuur**: geen e-mailcheck en geen melding als een factuur niet aankomt, geen postcode-naar-straat-aanvulling (2★, 2025-12-14). Bij een tweede reviewer zette een niet geregistreerde betaling een onterechte herinnering in gang.
- **Rapportage**: "Magere rapportering en statistieken die niet aanpasbaar zijn" (3★, 2026-08-10). Ook inzicht per leverancier of periode ontbreekt.
- **Vakbedrijf-functies ontbreken**: één (1★) reviewer, vermoedelijk technisch, mist "meerdere groothandels inladen… Geen agenda… geen werkbon mogelijkheid" (2026-07-28). Dit is een enkel geval, maar het past bij het profiel: WeFact is facturatie, geen vakmansoftware.
- **Monetisatie**: werkbonnen, opdrachtbevestiging en automatische offerte-opvolging zitten alleen in Plus (+€ 10 p/m). Middenreviewers zien dat als functies die achter een betaalmuur verdwijnen.

## Kansen voor ons CRM

- **Offerte-opvolging standaard, niet als betaalde add-on.** Bij WeFact zit automatische offerte-opvolging en "inzicht in geopende e-mails" in de Plus-laag, en de prijsstap wordt bekritiseerd. Opvolging (herinnering, "offerte geopend", pipeline) als kern van ons product is een duidelijk verschil. Onderbouwing: Plus-functielijst op de prijspagina en prijsklachten (13×).
- **Dossier per adres/klant met interne notities en bijlagen.** Het concrete gemis bij WeFact: een relatiedossier met alleen een "heeeel klein overzichtje" voor notities en geen interne bijlagen. Voor vakbedrijven (foto's, situatie ter plaatse) is dit essentieel.
- **Mobiel als volwaardige werkplek.** De WeFact-app is vooral om te kijken. Gebruikers willen vanaf de telefoon offertes maken, versturen en delen, met foto's (ook HEIC), handtekening en meerdere pagina's scannen. Voor de vakman op locatie is dit de lat.
- **Klantcommunicatie die bevestigt dat iets aankomt.** Voorbeelden: e-mailvalidatie en een bounce-melding bij offerte of factuur, adresaanvulling via postcode. Hier ligt een opening voor WhatsApp als kanaal met leesbevestiging. WhatsApp zelf wordt in deze reviews niet genoemd, dus dit is een afleiding.
- **Migratie en export als vertrouwensbelofte.** De FactuurSturen-saga laat zien hoe gevoelig "mijn administratie kwijt" en "data eruit halen kan niet" (lock-in 10×) liggen. Een eenvoudige import vanaf bestaande tools en een volledige export op elk moment zijn een verkoopargument.
- **Koppelen in plaats van vervangen.** Gebruikers waarderen de koppeling met boekhouder, bank, Mollie en Snelstart. Ons CRM hoeft geen facturatiepakket te worden. Het moet de offerte naadloos doorzetten naar WeFact, Moneybird of e-Boekhouden. WeFact heeft een API, maar één reviewer klaagt over "te strikte API limieten".
- **Lead-opvang en nazorg/onderhoud**: geen data in deze reviews, want WeFact doet dit niet. Periodieke facturen ("abonnementen") zijn het enige raakvlak met onderhoudscontracten. Juist die gaven bij de migratie veel problemen.
