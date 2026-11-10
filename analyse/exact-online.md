# Exact Online – review-analyse (gericht: facturatie, offerte, koppelingen, mobiel)

> Exact Online is een **algemeen boekhoud-/ERP-pakket**, geen vakbedrijf-CRM. Deze analyse is bewust smal: alleen reviews over offerte/facturatie, koppelingen (bank, Peppol, Zapier/API) en mobiel gebruik (de Exact Online-app). Reviews over fiscale modules, de nieuwe web-layout of algemene support zonder link met deze thema's zijn **niet** opgenomen. Bouw- en installatie-reviewers zijn in `reviewer_type` gemarkeerd. Het zijn er maar 3 (plus 1 "waarschijnlijk").

## Profielschets

- **Doelgroep**: mkb, zzp en accountantskantoren in NL/BE. Exact heeft ook een branchevariant "Exact voor Bouw" (exact.com/benl/producten/bouw) en is eigenaar van onder meer Bouw7 en Gripp. Die hebben aparte analyses in deze repo.
- **Prijsindicatie**: Onderneming.nl (laatst gecontroleerd 20-04-2026, via zoekresultaat van 10-11-2026) noemt Plus € 99 p/m en Essentials € 49 p/m (€ 588 per jaar). Finom noemt ook Professional € 159 en Premium vanaf € 299. Ik heb geen officiële Exact-prijspagina opgehaald, dus dit is een secundaire bron. Op Trustpilot klagen reviewers over meerprijzen: een upgrade van "140 euro per maand" alleen om 2 extra bankrekeningen te koppelen (2026-10-16), en betaalde koppelingen (2026-03-12).
- **Kernfuncties (relevant)**: verkoopfacturen en offertes, Peppol-e-facturatie, bankkoppelingen en betalen, inkoopfacturen en bonnen scannen, uren en kosten. Daarnaast de mobiele app (iOS id433619246, Android `com.exact`) met cockpit/dashboard, bonnen scannen, facturen goedkeuren, eenvoudige facturen maken, uren boeken en verlof.

## Databasis

| Bron | In CSV | 1★ | 2★ | 3★ | 4★ | 5★ | Opmerking |
|---|---|---|---|---|---|---|---|
| App Store NL | 37 | 22 | 9 | 3 | 1 | 2 | Uit de 100 nieuwste (2022-04 tot 2026-11). Alle reviews sinds nov. 2024 met inhoud, plus 4 oudere die over facturatie, CRM of een techniekbedrijf gaan. Loonstrook-/werknemer-reviews weggelaten |
| Google Play NL | 30 | 18 | 6 | 2 | 1 | 3 | Uit de 100 nieuwste (2022-03 tot 2026-11). Zelfde selectie, plus 3 oudere over facturatie |
| Trustpilot (NL-talig, exact.com) | 7 | 6 | – | – | 1 | – | Uit de 80 nieuwste NL-reviews (2026-02-11 tot 2026-11-10). Alleen de reviews over facturatie, koppelingen of de app, plus 1 bouwgebruiker |
| **Totaal** | **74** | | | | | | |

- **Verdeling (script `count.py`)**: 1 ster: 46 · midden: 23 · positief: 5. Sinds nov. 2024: 67 rijen (42 / 20 / 5). Er zijn 7 rijen van vóór nov. 2024; die zijn als "oud" te beschouwen.
- **Context Trustpilot**: de scraper meldt een TrustScore van 2,3 bij 717 reviews. In de 80 opgehaalde NL-reviews (54× 1★) gaat het grootste deel over **support/bereikbaarheid** (31 noemen support, helpdesk of klantenservice; trefwoord-telling met script). Verder:
  - prijs: 12
  - fiscale modules: 10
  - de nieuwe layout of gebruiksvriendelijkheid: 7
  - opzeggen/incasso na opzegging: 7

  Die thema's zijn alleen meegenomen als ze over facturatie, koppelingen of de app gaan. Een andere agent zag eerder veel Exact-reviews over prijsverhoging en opzeggen. Dat beeld klopt, maar die reviews gaan over Exacts eigen abonnement en niet over de facturatiefunctie.
- **Reviewer-type**: de meeste app-reviewers zijn ondernemers of zzp'ers die bonnen en facturen naar hun boekhouder sturen. Aantoonbaar bouw/installatie:
  - App Store 2026-11-02: installateur die offertes in Exact maakt
  - Trustpilot 2026-03-27: "exact online bouw"
  - App Store 2022-09-06: titel "BA Techniek Oost"
  - Google Play 2022-06-20: "btw verlegd"-factuur, waarschijnlijk bouw
- **Kwaliteitsnoot**:
  - Capterra.nl is niet opgehaald: de vermoedelijke reviewpagina (`/reviews/1014576/exact-for-finance`) gaf HTTP 410 of 404. Daarna niet verder gezocht, om zuinig te zijn met credits.
  - G2, Capterra.com en TrustRadius (12 reviews) zijn niet geprobeerd.
  - App-reviews zijn kort. Veel ervan zijn update-regressies (rond app-versie 6.0 in 2022, 7.0 in feb. 2025 en 7.1 in okt. 2025) en zeggen weinig over offerte/CRM.
  - Twee 5★-reviews bevatten toch een bug-melding. Het script telt ze als positief.

## Wat gebruikers goed vinden (de lat)

Weinig positieve reviews in deze selectie, maar wel duidelijk wat de app moet kunnen:
- **Snel inzicht onderweg**: "Snel en eenvoudig inzicht in de cijfers" (App Store, 2026-10-31). "Duidelijk de gegevens via de app, waar en wanneer je wil." (Google Play, 2025-08-29).
- **Bonnen scannen die netjes in de boekhouding landen**: "Heel makkelijk bonnen scannen of uploaden vanuit bestanden… (en daarna MOOI worden weergegeven in de boekhouding)" (Google Play, 2026-05-16).
- **Facturen delen vanuit mail of andere apps**: dit is de kernfunctie die gebruikers missen als hij stukgaat. "Voorheen was het ontzettend handig dat je facturen die vanuit andere apps moest halen met de delen functie naar de Exact app door kon sturen" (App Store, 2026-11-04).
- **Snel fixen wordt beloond**: "25-8 issue gefixt, dank Exact team voor zowel reply als fix!" (Google Play 5★, 2026-08-25).

## Top 5 pijnpunten

Frequentie is het aantal CSV-rijen met dat thema, uitgesplitst naar 1★ / midden / positief. Let op: `mobiel` zit in bijna elke rij, omdat het merendeel uit de app-stores komt.

| # | Thema | Frequentie (1★/midden/pos.) | Ernst |
|---|---|---|---|
| 1 | **bugs / stabiliteit in de app**: crashes, traag, uitloggen, regressies na updates | 53 (36/15/2) | Hoog: "app is nu feitelijk onbruikbaar" |
| 2 | **facturatie**: facturen uploaden, delen of goedkeuren in de app, Peppol, factureren via web | 27 (17/10/0) | Hoog: de kernflow (factuur maken, versturen, goedkeuren) valt weg |
| 3 | **support** dat het probleem niet oplost of de app niet kent | 9 (8/1/0) | Middel–hoog |
| 4 | **gebruiksgemak** van de app: omslachtig, verouderd, onhandig zoeken | 9 (4/5/0) | Middel |
| 5 | **koppelingen en prijs daarvan**: bank, betalen, Zapier, betaalde integraties | 5 (3/2/0); prijs 4 | Middel, maar relevant voor ons |

**1. Bugs en regressies in de app**
- "Barst van de bugs, lossen ze het ene op en creëren ze de volgende bug weer." (App Store, titel, 2026-11-02, installateur)
- "Loopt bij het invoeren van facturen continu vast… met het invoeren van 5 facturen ruim een half uur bezig" (Google Play, 2025-10-30)
- "Als ik de app opstart dan checkt hij mijn gezicht en crasht meteen." (App Store, 2026-09-24)

**2. Facturatie (in de app en web)**
- "Als je iets aanpast dan gaat hij random de omschrijving weer terug zetten naar \" consultancy per uur\" Ook vlak voor versturen" (App Store, 2026-09-14)
- "Al twee maanden lukt het niet om facturen voor een bepaalde klant via Peppol te versturen" (Trustpilot, 2026-10-22)
- "Het is niet meer mogelijk om een rekening te kopiëren voor een terugkerende klant" (App Store, 2026-08-20)

**3. Support**
- "De dame vd chat vd helpdesk wist mij te vertellen dat ze eigenlijk zelf de app nooit gebruikt" (Google Play, 2025-02-13)
- "In plaats van een oplossing wordt gesuggereerd om de kwestie als \"idee\" bij de developers neer te leggen" (App Store, 2026-08-20; niet in CSV-citaat, wel dezelfde review)

**4. Gebruiksgemak**
- "het is veel te omslachtig om even snel een bonnetje naar exact te sturen… in een paar (2) klikken" (Google Play, administratiekantoor, 2025-11-11)
- "lijkt net Windows 95" (App Store, 2026-04-13)

**5. Koppelingen**
- "De ervaring om exact te koppelen is dramatisch, overal moet je voor betalen… half werkende integratieoplossingen voor een premium prijs." (Trustpilot, 2026-03-12)
- "De koppeling met onze bank is nu een tijdje verbroken en ik wacht al bijna 1 maand" (Trustpilot, 2026-10-05)

## "Wat net mist" (middenreviews)

- **Notificaties en leesbaarheid op de telefoon**: "het zou handig zijn als er een notificatie is wanneer er iets binnenkomt. Dat gebeurt niet… Pinch zoom en schuiven werkt vrijwel niet." (App Store 2★, 2026-09-01). De functie bestaat wel, maar de mobiele uitvoering faalt.
- **Data in de app loopt achter op de desktop**: "wordt niet alles in de app goed geüpdatet nadat er facturen zijn verwerkt" (App Store 3★, 2026-02-05). Ook al in 2024: "de app update niet goed welke facturen betaald zijn, over datum zijn of nog open staan" (Google Play 2★, oud). Gebruikers willen op de telefoon een betrouwbare status per factuur.
- **De app als uitgeklede versie**: "Men kan niet àlles doen" (2024-11-11). Zoeken op relatie in plaats van op trefwoord is "Veelte omslachtig" (2025-10-21). Het btw-overzicht is weg (4★, 2026-02-11).
- **Werkbon en uren**: alleen indirect. "de app crasht regelmatig wanneer je gegevens zoals klant/ uren probeert in te vullen" (2026-07-22). Uit 2023 (oud, niet in CSV): de wens om dezelfde uren per dag te kopiëren.
- **Installateur-perspectief**: de enige expliciete installateur noemt het "voor installatiebedrijven het meest onvriendelijke boekhoud programma… niet alleen een programma is voor Boekhouders" (2026-11-02). Het boekhoudpakket wordt ook voor offertes gebruikt, maar is daar niet voor gemaakt.

## Kansen voor ons CRM

- **Offerte → factuur hoort in het vakman-CRM, niet in het boekhoudpakket.** De installateur-review en de Digitale Factuur-review ("oude offerte… opzoeken… kan dus niet", 2026-04-01) laten zien dat een boekhoudpakket het offerte-dossier slecht ondersteunt. Ons klantdossier per adres moet offerte, akkoord en factuur bij elkaar houden. Exact moet daarbij alleen de boekhoudkant afnemen, via een **koppeling naar Exact Online** die gratis en goed gedocumenteerd is. Dat is een verkoopargument, want reviewers ergeren zich juist aan betaalde en half werkende integraties.
- **Mobiele basisflows moeten na elke update werken.** Het grootste cluster klachten zijn regressies: delen of uploaden vanuit mail of andere apps, camera, goedkeuren. Voor ons betekent dat:
  - foto of PDF vanuit WhatsApp of mail via het share-menu naar het dossier;
  - automatische tests op deze flows;
  - releasenotes.
- **Status per factuur en offerte op de telefoon, actueel**: open, vervallen, betaald, gelezen, en een notificatie als er iets binnenkomt. Dat sluit direct aan op offerte-opvolging.
- **Terugkerende klant snel opnieuw factureren of offreren** (kopiëren). Dat past bij nazorg/onderhoud: dezelfde klant en hetzelfde adres elk jaar.
- **Btw-verlegd en Peppol goed regelen** in de factuurflow voor onderaannemers. Het signaal is dun (1 oude review en 1 Peppol-review), maar het faalt hard.
- **Support die de app zelf kent**: een gebruiker hoorde van de chat dat de medewerker de app nooit gebruikt. Een klein team dat zelf de app gebruikt is hier een onderscheidend punt.
