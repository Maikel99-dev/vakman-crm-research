# e-Boekhouden.nl – review-analyse (prioriteit 2)

> Focus: alleen offerte/facturatie, koppelingen en mobiel gebruik. Zuiver boekhoudkundige klachten (inkoopfacturen herkennen, btw, grootboek, jaarrekening) zijn weggelaten tenzij ze over koppelingen gaan. e-Boekhouden.nl is een **generiek online boekhoudpakket** (zzp, mkb, verenigingen). **Geen reviewer is herkenbaar als bouw-, installatie- of vakbedrijf**; herkenbare typen zijn een photobooth-verhuurder, een boekhouder, verenigingen en een penningmeester. **De data over offertes en koppelingen is dun** – lees dit als indicatie.

## Profielschets

- **Wie/wat**: e-Boekhouden.nl, Nederlands online boekhoudprogramma voor ondernemers, accountants en verenigingen/stichtingen. Functies (prijspagina): facturen in eigen huisstijl, offertes, abonnementen (terugkerende facturen), urenregistratie → factuur, herinneringen/aanmaningen, iDEAL/Wero-betaallink, UBL, relatiebeheer met eigen invoervelden, nieuwsbrieven, API en "koppelingen met externe systemen", mobiele app.
- **Prijsindicatie** (https://www.e-boekhouden.nl/prijzen, opgehaald 2026-11-10, per maand): **ZZP € 9,95** (max. 240 boekingen per boekjaar, onbeperkt factureren), **Standaard € 14,50** (onbeperkt boeken, **zonder factureren**), **Standaard + Factureren € 24,00**. Welkomstactie: starters 15 maanden gratis, anderen 12 maanden 50% korting. Mail & Herken-credits vanaf € 0,09.
- **Let op voor vakbedrijven**: wie facturen én onbeperkt wil boeken, zit op € 24 p/m; offertes zitten in de facturatiefunctie.
- **Apps**: iOS (id1078225120) en Android (eboekhouden.nl).

## Databasis

| bron | in CSV | wat opgehaald |
|---|---|---|
| Google Play NL (eboekhouden.nl) | 18 | 100 nieuwste reviews (2021-04 t/m 2026-10) via `thewolves/google-play-reviews-scraper` |
| App Store NL (id1078225120) | 9 | alle 72 beschikbare reviews (2016–2025), waarvan **maar 3 van na 2023**, via `thewolves/appstore-reviews-scraper` |
| Trustpilot (nl.trustpilot.com/review/www.e-boekhouden.nl) | 13 | Profiel: **2.069 reviews, TrustScore 4,5**, "297 reviews in de afgelopen 12 maanden". Gefilterde pagina 2–3★ (1 pagina, 20 reviews) via web-fetch + 18 reviews via `automation-lab/trustpilot` (vooral Engels, deels oud) |
| **Totaal** | **40** | |

- **Verdeling** (script over `data/e-boekhouden.csv`): 1 ster 6 · midden 27 · positief 7
- **Periode**: 2019-11 t/m 2026-10; **25 van 40 rijen van na nov 2024**. 15 oudere rijen (vooral app-reviews 2019–2023) zijn meegenomen omdat de recente app-data dun is; in de citaten gemarkeerd.
- **Kwaliteitsnoten**:
  - Trustpilot is overwegend positief (4,5). De middenreviews op Trustpilot gaan vooral over gebruiksgemak, verouderde interface en boekhoudkundig handwerk; **offertes worden in geen enkele kritische review genoemd**.
  - De App Store-reviews zijn grotendeels oud; de app lijkt daar weinig recente reviews te krijgen.
  - **Niet opgehaald**: Capterra/GetApp (WebSearch toonde een GetApp-vermelding; niet opgehaald om credits te sparen), Trustpilot 1★ en 4★-filters (niet opgehaald; de actor leverde slechts 18 reviews).

## Wat gebruikers goed vinden (de lat)

1. **Snel en eenvoudig factureren**, ook vanaf de telefoon: "Super goeie app snel en professioneel binnen minuut factuur klaar" (Google Play, 5★, 2022-03-13; oud). "Ideaal, je boekhouden, offertes en faktureren zijn met E-boekhouden kinderspel" (Google Play, 5★, 2026-04-12).
2. **Betaallink op de factuur**: "Op de factuur staat een iDeal-betaallink." (App Store, 5★, 2023-04-26; photobooth-verhuur)
3. **Bereikbare, menselijke support** (in tegenstelling tot Moneybird): "Klantenservice is snel, uitgebreide tutorials" (Trustpilot, 3★, 2026-07-04); een Italiaanse gebruiker roemt telefonische hulp (Trustpilot, 5★, 2026-10-02).
4. **Samenwerken met de accountant/boekhouder**: "Goede samenwerking met accountant mogelijk en facturen maken gaat netjes en gemakkelijk." (Google Play, 5★, 2024-03-18)

## Top 5 pijnpunten

| # | thema | freq. (1★/midden) | ernst | toelichting |
|---|---|---|---|---|
| 1 | mobiel (app = fractie van web) | 20 (5/15) | middel–hoog | weinig functies, verouderd, crashes bij opslaan |
| 2 | gebruiksgemak / verouderde UI | 14 (2/12) | middel | "10 jaar niet ge-updated", omslachtig voor niet-boekhouders |
| 3 | facturatie-details | 13 (2/11) | middel | factuuropmaak met codes, 2 decimalen, geen betaald-status in lijst |
| 4 | bugs (app) | 6 (1/5) | middel | app sluit af bij opslaan/factuur maken |
| 5 | koppelingen / import | 4 (0/4) | middel | koppelingsfout → 445 boekingen handmatig; import tussen accounts handmatig |

**1. Mobiel**
- "App biedt maar fractie van website… GUI van app en website behoorlijk verouderd, hoop gescroll." (Google Play, 2★, 2025-01-26)
- "Waarom kan ik mutaties niet inboeken in mijn telefoon?" (App Store, 2★, 2024-09-06; net buiten 24 mnd)
- "Heel irritant dat ik geen meldingen kan ontvangen van bijv. Facturen die overdatum zijn" (Google Play, 2★, 2024-11-04)

**2. Gebruiksgemak**
- "eigenlijk in 10 jaar niet ge-updated." (Trustpilot, 3★, 2025-01-15)
- "voor ondernemers zonder boekhoudkundige achtergrond is het erg ingewikkeld." (Trustpilot, 3★, 2025-02-15; boekhouder)

**3. Facturatie-details**
- "niet met codes [vrij1], [vrij2] waarbij het ook spannend blijft of het allemaal wel doorkomt" (Trustpilot, 2★, 2026-04-16)
- "alle facturen afgekeurd door de opdrachtgever omdat de decimale bij e-bookhouden twee achter de komma is" (Trustpilot, 3★, 2026-04-13)
- "Een groot gemis is om snel te zien in je facturen lijst of ze betaald zijn" (Google Play, 3★, 2025-04-27)

**4. Bugs**
- "App sluit constant af als ik iets wil opslaan. Ergernis!" (Google Play, 2★, 2026-04-10)

**5. Koppelingen**
- "Door een fout in een koppeling moet ik 445 boekingen aanpassen… Geen bulk edit." (Trustpilot, 2★, 2026-04-13)
- "Koppeling met andere programma's kan beter. Is ingewikkeld en hulp daarbij beperkt." (Google Play, 4★, 2021-12-10; oud)

## "Wat net mist" (uit middenreviews)

- **Factureren ter plekke bij de klant** met vooraf ingestelde producten – al jaren gevraagd: "als je bij een klan staat je direct een factuur kunt maken met je vooraf ingestelde producten" (App Store, 2★, 2019; oud) en "uren kan factureren in de app" (App Store, 4★, 2022; oud).
- **Inkoopregels doorzetten naar verkoop met marge** (Google Play, 4★, 2026-01-23) – dat is precies de materiaal-doorbelasting van een vakbedrijf.
- **Push-meldingen** bij vervallen facturen (2★, 2024-11) en een **betaald/onbetaald-status** in de factuurlijst.
- **WhatsApp/sms vanuit het klantcontact** in de app (Google Play, 4★, 2021-07; oud, enkel geval).
- **Visuele factuur-editor** in plaats van codes.

## Kansen voor ons CRM

- **Offerte en factuur maken op locatie met vaste producten/materialen en marge** – het meest concrete "wat net mist"-punt; e-Boekhouden lost het in de app niet op.
- **Opvolging met meldingen**: push bij vervallen facturen en (voor ons) bij openstaande offertes; de app biedt dat niet.
- **WhatsApp vanuit het klantdossier**: één (oude) reviewer vraagt er letterlijk om; onderbouwing zwak.
- **Stabiele koppeling naar e-Boekhouden** (API bestaat): veel kleine ondernemers en hun boekhouders zitten hierop. Koppelingsfouten kosten gebruikers uren handwerk zonder bulkcorrectie; een robuuste, controleerbare sync (met foutmelding vóór het boeken) is een verkoopargument.
- **Menselijke support als lat**: e-Boekhouden wordt gewaardeerd om bereikbare support; dat is het niveau dat vakmensen verwachten.
- **Lead-opvang, klantdossier per adres, nazorg/onderhoud**: geen data. Abonnementen (terugkerende facturen) zijn het enige raakvlak met onderhoudscontracten.
