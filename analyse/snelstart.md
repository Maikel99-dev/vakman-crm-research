# SnelStart – review-analyse (prioriteit 2)

> Focus: alleen offerte/facturatie, koppelingen en mobiel gebruik (SnelStart-app). Zuiver boekhoudkundige klachten (inlezen van inkoopfacturen, btw, vreemde valuta, jaarcijfers) zijn weggelaten tenzij ze over koppelingen gaan. SnelStart is een **generiek boekhoudpakket** voor mkb (vaak op advies van de boekhouder). **Herkenbaar uit de vakhoek zijn maar twee reviewers**: één die met **btw verlegd** factureert (typisch voor onderaanneming in de bouw; 2021, oud) en één die de app "in het veld" gebruikt en klanten op adres wil zoeken (2026). Verder geen branche-informatie.

## Profielschets

- **Wie/wat**: SnelStart Software B.V. (Alkmaar, sinds 1982). Boekhouding met facturatie en offertes, desktopversie (Windows) plus web/online-omgeving (de opvolger "Polaris" is volgens een reviewer nog in ontwikkeling), mobiele app voor bonnen, facturen en inzicht. API beschikbaar, maar alleen in hogere pakketten.
- **Prijsindicatie**: de prijspagina snelstart.nl/prijzen gaf een 404 (opgehaald 2026-11-10). Secundaire bronnen: ABN AMRO-partnerpagina noemt **inKaart € 22 p/m** (1 gebruiker, extra gebruiker € 4,25) en inOrde € 9,50 p/m (via WebSearch, niet zelf opgehaald). Een Trustpilot-reviewer (2026-09-09) noemt dat **API-toegang een upgrade van € 22 naar € 54 p/m plus € 250 certificeringskosten** vereist; een penningmeester noemt € 22 p/m (2026-11-02).
- **Apps**: iOS "SnelStart Boekhouden" (id1189100644), Android (nl.snelstart.web).

## Databasis

| bron | in CSV | wat opgehaald |
|---|---|---|
| App Store NL (id1189100644) | 19 | 100 nieuwste (2020-10 t/m 2026-09) via `thewolves/appstore-reviews-scraper` |
| Google Play NL (nl.snelstart.web) | 20 | 100 nieuwste (2023-09 t/m 2026-11) via `thewolves/google-play-reviews-scraper` |
| Trustpilot (nl.trustpilot.com/review/snelstart.nl) | 10 | Profiel: **2.296 reviews, TrustScore 4**, "460 reviews in de afgelopen 12 maanden". Gefilterde pagina 2–3★ (1 pagina, 20 reviews) via web-fetch; reviews over alleen inlezen/valuta/jaarwerk niet opgenomen |
| **Totaal** | **49** | |

- **Verdeling** (script over `data/snelstart.csv`): 1 ster 13 · midden 31 · positief 5
- **Periode**: 2021-02 t/m 2026-11; **36 van 49 rijen van na nov 2024**. 13 oudere app-reviews (vooral over offertes/facturen in de app) zijn meegenomen en in de citaten gemarkeerd.
- **Kwaliteitsnoten**:
  - De app-reviews worden sterk gedomineerd door **inlogproblemen** (Face ID/pincode vervallen na update aug–sep 2024, steeds opnieuw inloggen, wit scherm). Inhoudelijke feedback op factureren en offertes in de app is schaars.
  - Twee 5★-app-reviews bevatten een klacht (opgelost na herinstallatie; verzoek om QR-betaalcode); ze tellen als positief maar de thema's zijn wel gecodeerd.
  - **Niet opgehaald**: officiële prijspagina (404), Trustpilot 1★/4★-filters (credits), Capterra/G2 (niet gezocht om credits te sparen).

## Wat gebruikers goed vinden (de lat)

1. **Boekhouding en facturen grotendeels op de telefoon**: "Heel fijn dat ik mijn boekhouding grotendeels op mijn telefoon kan doen. Heel gebruiksvriendelijk." (Google Play, 5★, 2025-07-03). "ook niet de dwang van ik moet naar huis om bij de laptop te zijn." (Google Play, 5★, 2026-06-11)
2. **Facturen maken in de app** (als hij werkt): "Voor de rest een top app om facturen te maken duidelijk en overzichtelijk." (App Store, 3★, 2024-02-21). "het eenvoudig met de mobiel facturen en bonnen in het systeem zetten is super." (Google Play, 3★, 2024-05-17)
3. **Telefonische helpdesk is inhoudelijk goed** (maar slecht bereikbaar): "De hulp die geboden wordt is wel goed." (Trustpilot, 3★, 2026-05-20)

## Top 5 pijnpunten

| # | thema | freq. (1★/midden) | ernst | toelichting |
|---|---|---|---|---|
| 1 | mobiel (app onbetrouwbaar) | 28 (12/15) | hoog | inloggen mislukt, wit scherm, app valt weg |
| 2 | bugs/stabiliteit | 23 (10/12) | hoog | vooral login en uploads; jaren terugkerend |
| 3 | facturatie-details | 12 (3/7) | middel | €0,01 afrondingsverschil incl. btw, geen aanmaning, factuurvoorbeeld onleesbaar op telefoon |
| 4 | support-bereikbaarheid | 8 (3/5) | middel | lange wachttijden telefoon, terugbelverzoeken genegeerd |
| 5 | koppelingen & prijs (API/bank achter duurder pakket) | 6 koppelingen, 7 prijs | middel–hoog voor ons | API pas vanaf € 54 p/m + certificering; SumUp/Knab/Rabo haperen |

Ook: gebruiksgemak/verouderd 8×, offerte (in de app) 3×.

**1. Mobiel**
- "Inloggen in de app is 9 van de 10 keer dramatisch." (App Store, 1★, 2025-02-13)
- "Er wordt altijd gevraagd of ik naar de website wil. Wat is dan het nut van de app?" (Google Play, 1★, 2024-08-26)
- "Bij iedere bon en of maken van factuur opnieuw inloggen." (App Store, 2★, 2024-08-21)

**2. Bugs**
- "hij start nooit in 1x op, altijd 2* nodig" (Google Play, 3★, 2026-09-11)
- "Loopt continu tijdens de uploads vast, en wil niet inloggen. de normale internetversie heeft dit niet." (Google Play, 1★, 2025-09-09)

**3. Facturatie**
- "als je een factuur incl btw maakt staat er elke keer €0,01 erbij… Al jaren bezig met snelstart om dit gewijzigd te krijgen" (App Store, 2★, 2026-09-13)
- "Helaas je kan geen aanmaning sturen!" (App Store, 1★, 2026-08-19)
- "Niet optimized voor telefoon, factuur voorbeeld is echt om te janken." (Google Play, 1★, 2024-01-08)

**4. Support**
- "De laatste maanden moet je standaard een half uur wachten op hulp." (Trustpilot, 3★, 2026-05-20)

**5. Koppelingen/API**
- "Voor een API-koppeling naar je eigen gegevens moet je verplicht upgraden van 22 naar 54 euro per maand… 250 euro certificeringskosten" (Trustpilot, 2★, 2026-09-09). Dezelfde reviewer: bij e-Boekhouden is "token aanmaken self-service en duurt een minuutje".
- "ze rekenen wel veel geld voor API-koppelingen" (Trustpilot, 2★, 2026-08-16)
- "Ik mis een koppeling met SumUp." (Trustpilot, 3★, 2026-09-03)

## "Wat net mist" (uit middenreviews)

- **Klant zoeken op adres/woonplaats in de app** – letterlijk een vakman-behoefte: "Zeker de app in het veld is daarin niet geschikt. Enkel op naam zoeken in plaats van ook op adres of woonplaats." (App Store, 3★, 2026-04-01)
- **Factureren met marge in-/verkoop in de app** (App Store, 4★, 2022; oud) – materiaaldoorbelasting.
- **Offertes downloaden/mailen vanuit de app** werkt niet op iPad; offertes maken "gaat niet heel lekker" (Google Play, 3★, 2024-04-01).
- **QR-betaalcode op de factuur** zonder aparte Mollie-koppeling (App Store, 5★-met-wens, 2025-07).
- **Betaalbare koppelingen**: middenreviewers willen automatiseren (facturen klaarzetten via API, SumUp, bank), maar lopen tegen pakket-upgrades aan.

## Kansen voor ons CRM

- **Klantdossier per adres** met zoeken op adres/postcode in de mobiele app – de enige expliciet vakman-gerelateerde wens in deze dataset, en precies onze kern.
- **Koppeling naar SnelStart is duur voor de klant**: API-toegang vereist volgens een reviewer het € 54-pakket plus € 250 certificering. Voor ons CRM betekent dit: (a) koppeling met SnelStart kan voor de vakman een verborgen meerprijs zijn – vermeld dat eerlijk; (b) overweeg een export/UBL-route (factuur als UBL/Peppol naar het boekhoudpakket) als goedkoop alternatief. Te verifiëren bij SnelStart zelf.
- **Betrouwbaar inloggen (biometrie, sessie onthouden)** is basishygiëne die SnelStart al twee jaar niet op orde heeft; voor een vakman op de bouwplaats is "app opent niet" fataal.
- **Offerte en factuur op de telefoon die er óók op de telefoon goed uitzien** (preview, versturen, downloaden) – nu een zwakte.
- **Lead-opvang, WhatsApp, offerte-opvolging, nazorg/onderhoud**: geen data in deze reviews.
