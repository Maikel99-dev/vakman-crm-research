# HubSpot – review-analyse (alleen bouw / installatie / field service)

> **Zeer dunne data.** HubSpot is een algemeen sales- en marketingplatform. Ik heb alleen reviews opgenomen van reviewers in bouw, installatie of facilitaire dienstverlening. In de 100 nieuwste Capterra.com-reviews waren dat er **4**. Daarnaast is er **1** forumpost van een eigenaar van een klein dakdekkers-/bouwbedrijf. Ik heb niet aangevuld met algemene reviews. Alles hieronder is indicatief, niet representatief.

## Profielschets

- **Doelgroep**: B2B-sales- en marketingteams van elke omvang. Er is een gratis CRM met betaalde "Hubs" (Sales, Marketing, Content, Service). HubSpot heeft een eigen marketingpagina voor construction, maar geen branchesjabloon (zie forum hieronder).
- **Prijsindicatie** (secundaire vergelijkingssites via zoekresultaat, opgehaald 10-11-2026; niet geverifieerd op hubspot.com):
  - Sales Hub Starter ca. $7–20 per seat per maand, afhankelijk van de bron;
  - Professional ca. $90 per seat per maand plus een eenmalige onboardingfee van ca. $1.500.
  - Capterra-reviewers noemen de prijssprong bij groei als hoofdbezwaar.
- **Kernfuncties (relevant)**:
  - contacten en bedrijven, deals/pipeline;
  - offertes (quotes) in Sales Hub;
  - e-mailintegratie en -tracking, sequences, workflows;
  - formulieren en website (lead-opvang);
  - mobiele app;
  - marketplace met koppelingen, onder meer QuickBooks.

## Databasis

| Bron | In CSV | Sterren | Opmerking |
|---|---|---|---|
| Capterra.com (HubSpot CRM, 100 nieuwste reviews, okt. 2025 – nov. 2026, actor `azzouzana/capterra-reviews-scraper`) | 4 | 5, 4, 4, 3 | Industry = Construction (3×) en Facilities Services (1×). Eén review is via Software Advice gesyndiceerd. De andere 96 vielen in andere branches en zijn niet opgenomen |
| HubSpot Community (forum, 2025-06-25) | 1 | – | Vraag van de eigenaar van een "small but growing construction/roofing company". De antwoorden zijn van HubSpot-partners en consultants en zijn **niet** als review opgenomen |
| **Totaal** | **5** | | |

- **Verdeling (script)**: 1 ster: 0 · midden: 3 · positief: 1 · zonder score: 1. Alles is van na nov. 2024.
- **Kwaliteitsnoot**:
  - De 4 Capterra-reviews zijn kort en Engelstalig, waarschijnlijk van Amerikaanse bedrijven. Geen enkele reviewer komt uit NL en geen enkele is een kleine installateur.
  - G2 is niet geprobeerd voor HubSpot. Eén G2-poging (voor Pipedrive) gaf een time-out en G2 was eerder ook al niet op te halen.
  - De Capterra.com-reviewpagina zelf gaf via web-fetch een time-out, daarom is de scraper gebruikt.
  - De Software Advice-pagina "construction/hubspot-profile/reviews" gaf 404.
  - Op Reddit zocht ik via WebSearch, maar vond ik alleen blogs van concurrenten die Reddit citeren. Die zijn niet opgenomen.
  - Een tweede Capterra-run (bijv. sortering "lowest rated") is niet gedaan vanwege de regel van max. 100 items per bron.

## Wat gebruikers goed vinden

- **Alles bij elkaar, eenvoudig**: "I like that all of the information needed is stored together" (Estimating Coordinator, construction 51-200, 5★, 2026-03-25).
- **Leads, gesprekken en opvolging overzichtelijk, met e-mailintegratie**: "helps me keep track of leads, client conversations, and follow-ups without adding unnecessary complexity" en "integrates smoothly with email, making it easy to track communication history" (VP of Sales and Estimating, construction 11-50, 4★, 2026-01-20).
- **Klanten filteren op type of locatie**: "I am able to sort clients by type, location, and even job title" (Facilities Services, 3★, 2025-11-07).

## Top pijnpunten (n = 5, alleen indicatief)

| # | Thema | Frequentie | Ernst |
|---|---|---|---|
| 1 | **prijs**: duur bij groei, functies achter hogere tiers | 3 | Hoog: de eigenaar van een bouwbedrijf (11-50) is erom vertrokken |
| 2 | **onboarding / te complex**: geen branchesjabloon, gevoel van geld verspillen | 1 (forum) | Hoog voor kleine bedrijven |
| 3 | **rapportage / automatisering** alleen in hogere tiers | 1 | Middel |
| 4 | **gebruiksgemak**: automatisch uitloggen en 2FA bij elke login | 1 | Laag |
| 5 | **datakwaliteit** van verrijkte contactgegevens | 1 | Laag (prospecting, minder relevant voor ons) |

- Prijs: "I found it very expensive to grow with, which is very bad. HubSpot seems built only for big companies, and small businesses can’t afford it" (Owner, construction 11-50, 4★, 2026-09-22, titel "We can’t afford it anymore").
- Onboarding: "we’re paying quite a lot per month (Sales, Marketing, and Content Hub Pro), but I honestly feel lost on how to use it properly… We feel like we’re wasting money on a powerful system we don’t know how to use." (forum, 2025-06-25). De vragensteller wil onder meer verzekeringsklussen van begin tot eind volgen, winst per klus bijhouden en leads organiseren. Hij vraagt: "Is there a template or playbook for contractors?"
- Tiers: "Some advanced reportings and automation features are limited unless you move to higher-tier plans" (2026-01-20).

## "Wat net mist" (middenreviews)

- **Betaalbaar meegroeien**: de 4★-eigenaar vond het "affordable and worked well at first". Het probleem ontstaat pas bij de volgende tier.
- **Branchelogica zit niet in het product**: klusfases, verzekeringsclaims en winst per klus moeten via custom pipelines en properties worden gebouwd, en de klant moet daarvoor een partner inhuren. Dit komt uit de forumvraag; de partnerantwoorden zijn geen reviews.

## Kansen voor ons CRM

- **Vooringerichte pipeline voor vakbedrijven** (aanvraag → opname → offerte verstuurd → akkoord → ingepland → uitgevoerd → betaald → nazorg). Zo hoeft de klant niet "lost" te zijn of een consultant in te huren.
- **Voorspelbare, vlakke prijs voor 2–25 man.** Dat is het meest genoemde pijnpunt, ook bij een tevreden gebruiker.
- **E-mail (en WhatsApp) automatisch in het klantdossier.** Dat is precies wat de estimators waarderen.
- **Winst per klus / koppeling met boekhouding** als basis, niet als maatwerk.
