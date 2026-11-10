# Review-analyse software voor technische vakbedrijven (NL)

Onderzoek naar wat Nederlandse technische vakbedrijven (2–25 man: dakdekkers, installateurs,
schilders, kleine aannemers) goed en níét goed vinden aan bestaande software, als input voor een
verticaal CRM (aanvragen opvangen, offertes maken + opvolgen, klantdossier per adres, nazorg/onderhoud).

## Structuur

- `data/<tool>.csv` – ruwe reviews (één rij per review/post)
- `analyse/<tool>.md` – analyse per tool
- `SAMENVATTING.md` – markt-brede synthese

## CSV-formaat

Kolommen: `tool,bron,url,datum,sterren,reviewer_type,tekst,themas`

Uitzondering: `data/werkspot.csv` heeft een extra kolom `reviewer_kant` (vakman/consument/onbekend) na `reviewer_type`.

- `datum`: ISO (`YYYY-MM-DD`), of `YYYY-MM` / `YYYY` als alleen dat bekend is; leeg als onbekend
- `sterren`: 1–5 (Capterra/G2 omgerekend naar 5 als nodig); leeg voor forumposts/comments zonder score
- `reviewer_type`: rol/branche/bedrijfsgrootte als bekend (bv. "installateur, 2-10 medewerkers"), anders leeg
- `tekst`: kort en letterlijk (of ingekort met `…`), max ~40 woorden. Nooit verzonnen.
- `themas`: codes uit het codeboek hieronder, gescheiden door `;`

## Codeboek thema's

| code | betekenis |
|---|---|
| onboarding | onboarding / implementatie / inrichting |
| gebruiksgemak | gebruiksgemak / UI / leercurve |
| mobiel | mobiele app / offline gebruik |
| offerte | offerte maken |
| offerte-opvolging | offerte-opvolging / pipeline / herinneringen |
| planning | planning / agenda |
| werkbon | werkbon / urenregistratie op locatie |
| facturatie | facturatie / koppeling boekhouding |
| klantcommunicatie | klantcommunicatie (WhatsApp/sms/mail) |
| lead-opvang | lead-opvang / aanvragen binnenhalen |
| rapportage | rapportage / inzicht |
| prijs | prijs / prijsverhoging / prijsmodel |
| support | support / klantenservice |
| bugs | bugs / stabiliteit / snelheid |
| ontbrekend:<functie> | ontbrekende functie, bv. `ontbrekend:voorraad` |
| lock-in | lock-in / data-export / opzeggen |
| koppelingen | overige koppelingen / API (niet-boekhouding) |
| leadkwaliteit | (leadplatforms) kwaliteit / echtheid van leads |
| leadkosten | (leadplatforms) kosten per lead / abonnement / geld terug |
| positief:<onderwerp> | expliciete waardering, bv. `positief:support` |

## Groepen

- **1 ster**
- **midden**: 2–3 sterren + kritische 4-sterren (4 sterren mét concreet klachtpunt)
- **positief**: 4–5 sterren zonder wezenlijke klacht

## Bronbeperkingen in deze onderzoeksomgeving

Directe toegang tot Trustpilot, Capterra, Google Play en de App Store is vanuit de sandbox
geblokkeerd; reviews zijn opgehaald via Apify-scrapers en -web-fetch. Pagina's die niet op te halen
waren staan per tool genoteerd in de kwaliteitsnoot.
