# Tradecount – review-analyse

> **Resultaat: product niet te vinden, 0 reviews.** We konden niet vaststellen dat er een Nederlandse vakman-software "Tradecount" (tradecount.nl) bestaat: Apify kon het domein niet ophalen (502) en geen enkele zoekmachine levert een treffer op. Daarom is er geen analyse gemaakt. `data/tradecount.csv` bevat alleen de kopregel.

## Profielschets

Niet vast te stellen. Pogingen (2026-11-10):

| poging | resultaat |
|---|---|
| Apify web-fetch `https://tradecount.nl/` | timeout na 60 s |
| Apify web-fetch `https://www.tradecount.nl/` | HTTP 502 `UPSTREAM_FETCH_ERROR` ("Failed to fetch") |
| Ingebouwde WebFetch `https://tradecount.nl/` | `getaddrinfo ENOTFOUND`. Dit zegt niets: dezelfde fout trad ook op bij www.wefact.nl, dus de sandbox blokkeert de ingebouwde WebFetch gewoon. |
| Apify web-search "Tradecount app reviews" (NL) | alleen naamgenoten (Trade Cut, Tradetrak, Trade Counter Direct) |
| Apify web-search "\"Tradecount\" software vakman" (NL) | 0 resultaten |
| WebSearch "Tradecount vakman software tradecount.nl" | geen treffers; dichtstbijzijnde is "Transcount" (expeditiesoftware, ander product) |
| WebSearch "\"Tradecount\" app offerte factuur vakmensen" | geen treffers; wel andere vakman-tools (Bosch OfficeOn, Informer, Plancraft) |
| WebSearch "\"tradecount\" Nederland" | alleen handelsstatistieken (CBS/OEC) |

## Databasis

- Reviews: **0** (geen app, geen Trustpilot-, Capterra- of G2-profiel te vinden, want er is geen product om op te zoeken)
- App Store en Google Play: niet doorzocht met scrapers, omdat er geen app-ID of ontwikkelaarsnaam bekend is. Een scraper laten raden kost credits en levert niets bruikbaars op.

## Wat gebruikers goed vinden / Top 5 pijnpunten / "Wat net mist" / Kansen

Geen data, dus geen bevindingen.

## Aanbeveling

Ga na of de naam klopt. Mogelijk is iets anders bedoeld, zoals **Tradecraft**, **Tradify** (vakman-app uit Nieuw-Zeeland, ook in de Benelux), **Plancraft** of **Bosch OfficeOn**. Met de juiste naam of URL kan de analyse alsnog worden gedaan.
