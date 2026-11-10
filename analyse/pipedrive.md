# Pipedrive – review-analyse (alleen bouw / installatie / field service)

> **Dunne data.** Pipedrive is een algemeen sales-CRM. Ik heb alleen reviewers opgenomen met branche Construction (6), "Glass, Ceramics & Concrete" (1) of "Renewables & Environment" (2). Die kwamen uit de 100 nieuwste Capterra.com-reviews. Er is niet aangevuld met algemene reviews. Het is een kleine, overwegend positieve steekproef van vooral Engelstalige, niet-Nederlandse bedrijven.

## Profielschets

- **Doelgroep**: salesteams in kleine en middelgrote bedrijven. Pipedrive heeft een eigen pagina "CRM for construction" voor remodelers, aannemers en installateurs (elektro, HVAC, loodgieters).
- **Prijsindicatie** (secundaire vergelijkingssites via zoekresultaat, opgehaald 10-11-2026; niet geverifieerd op pipedrive.com): Lite $14, Growth $39, Premium $59 en Ultimate $79 per gebruiker per maand bij jaarbetaling. Maandelijks is het $24/$49/$79/$99. De plannen zijn in sept. 2025 hernoemd. Capterra noemt "starting price $19 per user per month" en een rating van 4,5 bij ca. 3.060 reviews.
- **Kernfuncties (relevant)**:
  - visuele deal-pipeline en activiteiten/herinneringen;
  - webformulieren en leadbooster (lead-opvang);
  - offertes/documenten (o.a. met Google-sjablonen);
  - e-mailsynchronisatie en e-mailmarketing (Campaigns);
  - marketplace-koppelingen, onder meer telefonie (JustCall);
  - mobiele app.

## Databasis

| Bron | In CSV | 1★ | 3★ | 4★ | 5★ | Opmerking |
|---|---|---|---|---|---|---|
| Capterra.com (Pipedrive, 100 nieuwste reviews, sept. 2024 – okt. 2026, actor `azzouzana/capterra-reviews-scraper`) | 9 | 1 | 1 | 3 | 4 | 6× Construction, 1× Glass/Ceramics/Concrete, 2× Renewables & Environment. De andere 91 zijn niet opgenomen. "Architecture & Planning" (1) is niet als bouw meegeteld |

- **Verdeling (script)**: 1 ster: 1 · midden: 4 · positief: 4. Sinds nov. 2024: 8 van de 9 rijen. De review van 2024-10-01 is net ouder.
- **Talen**: 7 Engels, 1 Italiaans, 1 Duits. Citaten staan in de originele taal.
- **Kwaliteitsnoot**:
  - G2 is één keer geprobeerd (web-fetch, gefilterde URL) en gaf een time-out. Daarna niet opnieuw geprobeerd.
  - Op Reddit vond ik via WebSearch geen first-hand contractor-threads over Pipedrive, alleen blogs van concurrenten (JobNimbus, Contractor+ e.d.). Die zijn niet opgenomen.
  - App Store en Google Play zijn niet geprobeerd. Daar staat geen branche bij de reviewer, dus ze voldoen niet aan het filter.
  - Geen NL-reviewers in deze set.

## Wat gebruikers goed vinden

- **Visuele pipeline met klusfases, geen gemiste opvolging**: "The visual pipeline is easy to use, keeps our team accountable, and ensures no follow-ups are missed." (Managing Director, construction 1-10, 5★, 2025-12-15). En: "different categories to separate stages of a job" (construction 51-200, 5★, 2026-05-04).
- **Prijs ten opzichte van branchesoftware**: een kantoormanager in construction stapte over omdat "Acculynx is very expensive, was looking for a cheaper CRM" (4★, 2025-04-09). Ook: "Overall satisfied when considering it is a low cost product" (Renewables, 3★, 2024-11-05).
- **Online offerte-aanvraag door de klant zelf**: "easy way to get online quotes. Customers can enter all there info online." (Glass/Concrete, 4★, 2025-05-16). **Offertesjablonen**: "Modello di preventivazione, intuitivo" (project manager, construction, 4★, 2025-05-03).
- **Herinneringen**: "erinnert mich fast automatisch an Termine und Erledigungen" (energieadviseur, 5★, 2024-10-01).

## Top pijnpunten (n = 9, indicatief)

| # | Thema | Frequentie | Ernst |
|---|---|---|---|
| 1 | **gebruiksgemak** in details: deal toewijzen bij aanmaken, zoeken/filteren, leercurve voor minder digitale collega's | 3 | Middel |
| 2 | **e-mailmarketing geblokkeerd** door herhaalde verificatie | 1 (1★) | Hoog voor die gebruiker |
| 3 | **ontbrekende branchefuncties**: voorraad, prijslijst | 1 | Middel |
| 4 | **onvolledige aanvragen** via online formulier | 1 | Middel, zeer relevant voor lead-opvang |
| 5 | **beperkingen bij meerdere productlijnen of vestigingen**, geen eigen telefonie | 2 | Laag–middel |

- "I don't like that you can't assign a job to a person as you make a pipedrive. It automatically puts it under your name" (2026-05-04)
- "My less-computer literate coworkers struggled to get the hang of it." (2025-04-09)
- "The platform verifies your company profile multiple times… During the verification process you can't proceed with your campaigns." (CEO, construction 11-50, 1★, 2025-11-16)
- "Sometimes customers do not enter all the information. They miss some important info." (2025-05-16)
- "gestione piu approfondita di un magazzino e listino prezzi" (2025-05-03)

## "Wat net mist" (middenreviews)

- **Aanvraagformulier dat volledige informatie afdwingt.** Klanten vullen de online offerte-aanvraag onvolledig in. Voor ons zijn dat verplichte velden per klustype, foto-upload en terugvragen via WhatsApp.
- **Medewerkers die minder digitaal zijn haken af.** De pipeline zelf wordt gewaardeerd, maar de leercurve voor "less-computer literate coworkers" blijft.
- **Prijslijst en artikelen in de offerte** ontbreken voor een bouwbedrijf (Italiaanse PM). Pipedrive is sterk in opvolging, zwak in de calculatiekant.
- **Prijsvoordeel tegenover vertical software** (AccuLynx) is een expliciete overstapreden. Kopers in de bouw vergelijken dus met branchetools op prijs.

## Kansen voor ons CRM

- **De lat voor offerte-opvolging ligt bij Pipedrive**: een visuele pipeline per klusfase en automatische herinneringen ("no follow-ups are missed"). Dat moet ons CRM minstens even simpel bieden.
- **Wat Pipedrive mist en wij kunnen bieden**:
  - offerte mét prijslijst/artikelen;
  - een aanvraagformulier en WhatsApp-intake die volledige informatie en foto's afdwingen;
  - klantdossier per adres;
  - eenvoud voor monteurs en minder digitale medewerkers.
- **Prijs**: bouwbedrijven stappen over van dure vertical tools naar Pipedrive vanwege de prijs. Een vakman-CRM moet in de buurt blijven van ca. $15–40 per gebruiker, of per bedrijf prijzen.
- Telefonie en e-mailmarketing zijn bij Pipedrive add-ons of koppelingen. Voor kleine vakbedrijven is het waarschijnlijk belangrijker dat WhatsApp en telefoon in het dossier landen dan dat er campagnes zijn. Dat is niet onderbouwd door deze reviews, dus het is een hypothese.
