# OutSmart – review-analyse

## Profielschets

- **Wat**: field-service-/werkbonsoftware (out-smart.com; voorheen "WerkbonApp"). Backoffice met planbord, plus de mobiele app (Android `com.werkbon`, iOS "OutSmart | Field Service"). Let op: outsmart.nl is van een ander bedrijf.
- **Doelgroep**: bedrijven met buitendienst: installateurs, service- en onderhoudsbedrijven, van zzp'er tot tientallen monteurs (één review noemt 95 tablets).
- **Kernfuncties**: digitale werkbon (uren, materialen, foto's, handtekening), planbord, objectbeheer/onderhoudshistorie, contracten/SLA, formulieren, facturatie, offertes (vanaf het Accelerate-pakket), koppelingen met Exact Online, AFAS, SnelStart, Moneybird, Yuki e.a.
- **Prijsindicatie** (via SoftwareWatcher, dat zegt de prijspagina van OutSmart op 5 okt 2026 gecontroleerd te hebben; opgehaald 10 nov 2026, excl. btw):
  Launch € 180/jaar (1 gebruiker); Boost € 448/jaar (2 gebr., +€ 224 per extra); Accelerate € 1.710/jaar (5 gebr., +€ 342; met offertes, objectbeheer, contracten); Maximize € 2.300/jaar (5 gebr., +€ 460). Een boekhoudkoppeling kost apart € 5,50–27,50 per maand (Exact € 27,50), plus "Power-Ups" per maand; implementatie en training zijn aparte pakketten. In reviews: implementatiepakket € 1.600 en € 300 voor een training van een half uur (Trustpilot, feb 2024). De eigen prijspagina (out-smart.com/nl/prijzen) gaf een 404, en /nl/nieuwe-tarieven (tarieven per 1 okt 2024) gaf geen tekst terug.

## Databasis

| bron | aantal in CSV | waarvan sinds nov 2024 |
|---|---|---|
| Google Play (com.werkbon, NL) | 40 | 16 |
| App Store NL (id1314341924) | 35 | 18 |
| Trustpilot (out-smart.com, alle reviews; TrustScore 2,3) | 22 | 11 |
| SoftwareWatcher.nl (zonder datum) | 3 | – |
| **Totaal** | **100** | **45** |

- **Verdeling**: 48 × 1 ster, 33 × midden (2–3 sterren + kritische 4–5 sterren), 19 × positief.
- **Periode**: dec 2021 – nov 2026. Uit de app-stores staan alleen reviews vanaf 2022 in de CSV. De scraper haalde er in totaal 226 (Play) en 73 (App Store) op. De ongeveer 150 oudere reviews (2014–2021) zijn weggelaten, maar ze laten hetzelfde patroon zien: crashes en verdwenen bonnen na updates. 55 rijen zijn ouder dan 24 maanden; die zijn meegenomen omdat het patroon gelijk blijft.
- **Groepsregel**: 4–5 sterren tellen als "positief" als alle thema's `positief:` zijn, anders als "midden". Eén 5-sterrenreview (App Store, jan 2025) is inhoudelijk een prijsklacht en valt daardoor onder midden.
- **Kwaliteitsnoot**:
  - App-reviews zijn vaak kort ("Werkt niet") en per app niet aan een vakgebied te koppelen. Trustpilot is lang en zakelijk, maar het zijn er weinig (22) en ze zitten geclusterd rond de prijswijziging van okt/nov 2024.
  - De SoftwareWatcher-scores (4,3 / 4,2 / 4,6) zijn afgerond naar 4/4/5.
  - De OutSmart Next-app (`com.outsmart.app`) leverde 0 NL-reviews op.
  - Capterra (UK) toont 0 reviews. Capterra.nl/G2 vond ik niet via zoeken.
  - Tweakers en Reddit: niets relevants gevonden.
  - Trustpilot outsmart.nl: geen profiel (ander bedrijf).
  - Google Maps-reviews heb ik niet geprobeerd.

## Wat gebruikers goed vinden (de lat)

- **De werkbon vervangt papier en komt professioneel over**: "Zeer tevreden ervan! En komt professioneel over tegen over mijn klanten!" (Google Play, feb 2022). "Scheelt mij heel veel administratie als zzp’er" (App Store, okt 2025).
- **Veel functies, in één keten**: "We hebben onze hele primaire proces van aanvragen op onze website tot aan de facturatie geautomatiseerd met Outsmart." (SoftwareWatcher). "Beste field Service app van alle die we geprobeerd hebben. Wij hebben het systeem gekoppeld aan Exact online." (App Store, mrt 2023)
- **Persoonlijke support, als je de juiste persoon treft**: "zeer behulpzame en kundige support afdeling" (Google Play, aug 2024). "Na klacht, direct contact en oplossing." (App Store, sep 2024). Goede onboarding plus een werkende ERP-koppeling (Trustpilot, apr 2025).
- **Formulieren buiten de werkbon**: "gebruiken voor het sales team, om opnameformulieren te maken, zodat op basis van deze informatie de offerte gemaakt kan worden" (App Store, mei 2023).

## Top 5 pijnpunten

| # | thema | frequentie (van 100) | 1 ster / midden | ernst |
|---|---|---|---|---|
| 1 | bugs / stabiliteit (crashes, data weg na updates) | 50 | 31 / 19 | hoog: werk gaat verloren, de monteur moet terug naar de klant |
| 2 | mobiele app (Android, full-screen, typen onzichtbaar) | 18 | 10 / 8 | hoog voor de buitendienst |
| 3 | werkbon/uren onbetrouwbaar (niet verstuurd, gegevens verspringen) | 17 | 7 / 10 | hoog: facturatie klopt niet |
| 4 | prijs / prijsverhoging (×3 tot ×4) + lock-in (8) | 13 (+8) | 12 / 1 | hoog: vertrouwen en churn |
| 5 | support slecht bereikbaar / tickets dichtgezet | 11 | 11 / 0 | hoog |

Daarnaast: gebruiksgemak (13), onboarding/implementatiekosten (6), planning (6) en boekhoudkoppeling (5: Exact, SnelStart, e-Boekhouden).

**1. Stabiliteit en data die verdwijnt**
- "werkbonnen en afspraken zijn plotseling weer verdwenen uit de agenda! superfijn als je onderweg bent" (Google Play, 2025-11-26, 2★)
- "verzonden bonnen de volgende dag weer in planbord staan echter helemaal leeg" (Google Play, 2024-02-15, 1★)
- "Regelmatig na een update van de app, loopt alles totaal niet zoals je zou moeten." (App Store, 2025-02-16, 1★)

**2. Mobiele app**
- "Op iPhone werkt het best goed, maar op Android echt slecht" (Google Play, 2026-11-06, 2★)
- "Sinds android 16 kan je inderdaad niet meer zien wat je aan het typen bent." (Google Play, 2025-09-23, 1★)
- "Loop eens een dagje met een monteur mee. Dit kan en moet zoveel logischer." (App Store, 2026-07-22, 2★)

**3. Werkbon/uren onbetrouwbaar**
- "soms worden de werkbonnen niet verstuurd via de email" (Google Play, 2025-10-16, 3★)
- "één van de andere werkzaamheden compleet spontaan veranderd … Hierdoor kloppen de bonnen niet meer" (Google Play, 2024-12-06, 1★)
- "loopt de app op mijn iPhone compleet vast wanneer ik mijn uren wil invullen" (App Store, 2026-08-15, 1★)

**4. Prijs en lock-in**
- "ga ik voor het zelfde product 4 keer zoveel betalen en dit is niet bespreekbaar" (App Store, 2025-01-11, eenmanszaak)
- "waardoor mijn prijs nu verdrievoudigd is" (Trustpilot, 2024-12-24, 1★)
- "dwingt gebruikers … van maandelijkse naar kwartaal- of jaarlijkse facturatie over te stappen. Slechts twee maanden aankondigingstijd" (Trustpilot, 2024-11-01, 1★)

**5. Support**
- "Onlangs heb ik na 1 uur en 41 minuten de moed opgegeven" (Trustpilot, 2024-01-31, 1★)
- "na 3/4 dagen krijg je pas reactie , en dan te weten dat de monteur ter plekke iets ontdekt wat niet werkt" (Trustpilot, 2024-11-03, 1★)
- "e-mails worden genegeerd en de telefonische bereikbaarheid is bijzonder slecht" (Trustpilot, 2026-01-06, 1★)

## "Wat net mist" (uit de middenreviews, n=33)

- **De boekhoudkoppeling werkt "net niet"**: "Op zich prima app, alleen de integratie met Exact Online werkt net niet. Iedere factuur moet met de hand worden bijgewerkt." Dezelfde klant schreef dit in jul 2026 op Google Play, de App Store en Trustpilot. Het systeem zelf vinden ze goed; handwerk aan facturen is de afknapper.
- **Bediening in het veld**: full-screen zonder navigatiebalk, een agenda die terugspringt, scrollen in plaats van tijden intypen, en voor elke foto eerst een "object" aanmaken. Middenreviewers zijn "over het algemeen blij", maar ergeren zich aan veel kleine handelingen.
- **Synchronisatie planning ↔ app**: bonnen die op kantoor zijn verwijderd blijven in de app staan, met "een ongewenst bezoek" als gevolg (App Store, mei 2025).
- **Kleine wensen**: een urenoverzicht per week, routeoptimalisatie en CarPlay.

## Kansen voor ons CRM

1. **Betrouwbaarheid als belofte**: offline-first, met lokaal opslaan per veld en nooit verlies van ingevulde data, plus een duidelijke status "verzonden naar kantoor / naar klant". Dit is het grootste en meest emotionele pijnpunt (50/100).
2. **Eerlijk, voorspelbaar prijsmodel**: maandelijks opzegbaar, zonder gedwongen pakketmigratie, met export zonder drempel. De prijswijziging van OutSmart in 2024 leverde een cluster 1-sterren op en klanten die actief zoeken naar een alternatief. Dat is een directe wervingskans. Doelgroep: kleine bedrijven en zzp'ers die ×3–4 gingen betalen.
3. **Klantdossier per adres/object**: objecthistorie wordt gewaardeerd, maar laadt niet ("je niet kunt zien wat de vorige problemen waren met de machine", App Store, okt 2022) of crasht (Play, nov 2024). Een snel, robuust dossier per adres met eerdere bonnen, foto's en installaties is een duidelijke kans voor nazorg en onderhoud.
4. **Lead-opvang en offerte-opvolging** komen in de OutSmart-reviews nauwelijks voor (één positieve vermelding van "aanvragen op onze website tot aan de facturatie"). Offertes zitten pas in het duurdere Accelerate-pakket. Dit ligt dus buiten de kern van OutSmart. Wij kunnen het in het instappakket stoppen, maar de reviews onderbouwen deze vraag niet direct.
5. **Klantcommunicatie**: de enige vermelding is dat werkbonnen niet per e-mail aankomen bij de klant. Betrouwbare verzending, eventueel via WhatsApp met leesbevestiging, sluit hierop aan. Het bewijs is dun (n=1).
6. **Support die het probleem ook echt oplost**: geen tickets laten sluiten als de klant niet reageert, en een vaste contactpersoon tijdens de eerste maanden (een concreet advies uit Trustpilot, jan 2024).
