# Moneybird – review-analyse (prioriteit 2)

> Focus: alleen offerte/facturatie, koppelingen en mobiel gebruik (app). Zuiver boekhoudkundige onderwerpen (btw-aangifte, jaarrekening, bonnetjes verwerken als boekhoudtaak) zijn bewust weggelaten, behalve waar ze de app-stabiliteit raken. Moneybird is **generiek boekhoud- en facturatiepakket voor zzp en mkb**, geen vakmansoftware. In de opgehaalde reviews is **geen enkele reviewer herkenbaar als bouw-, installatie- of vakbedrijf**. Lees dit als "de lat voor facturatie en de factuur-app bij kleine ondernemers".

## Profielschets

- **Wie/wat**: Moneybird B.V. (Enschede). Online boekhouding met facturen, offertes (met opties en digitale ondertekening, offerte → factuur met één klik), periodieke facturen, automatische herinneringen, online betaalmethoden, urenregistratie, eigen betaalrekening, API. Claimt "ruim 400.000 ondernemers" (prijspagina).
- **Bouw-pagina** (https://www.moneybird.nl/voor-wie/sectoren/bouw-en-installatietechniek/, opgehaald 2026-11-10): positioneert "een offerte maken tussen twee klussen door… vanaf je telefoon" en betalen op locatie. Genoemde koppelingen voor de bouw: **Woub** (bouw), **Nanda** en **Time On** (urenregistratie). Werkbon-/planningsoftware zoals Gripp, Tradecount e.d. wordt op die pagina niet genoemd.
- **Prijsindicatie** (https://www.moneybird.nl/prijzen/, opgehaald 2026-11-10, per maand bij jaarbetaling; maandbetaling tussen haakjes): Compact € 3 (€ 4; 1 verkoopfactuur, 5 transacties), Start € 15 (€ 18; 200 facturen, 20 transacties, 1 gebruiker, **geen externe bankkoppeling**), Groei € 29 (€ 35; 5 gebruikers, 5 gekoppelde banken), Compleet € 41 (€ 49; onbeperkt). Boven het factuurlimiet € 0,15 per extra factuur. 60 dagen gratis proberen. Het gratis pakket is in 2026 vervallen (bevestigd in Moneybird-reacties op Trustpilot).
- **Mobiel**: iOS-app "Moneybird - Boekhouding" (id1169487040) en Android-app (com.moneybird.android): facturen/offertes maken en versturen, bonnen scannen, bank, uren.

## Databasis

| bron | in CSV | wat opgehaald |
|---|---|---|
| App Store NL (id1169487040) | 25 | 100 nieuwste reviews (2021-12 t/m 2026-11) via `thewolves/appstore-reviews-scraper`; opgenomen zijn de reviews over factureren/offertes in de app, stabiliteit en mobiele beperkingen |
| Google Play NL (com.moneybird.android) | 19 | 100 nieuwste (2023-01 t/m 2026-10) via `thewolves/google-play-reviews-scraper`; zelfde selectie |
| Trustpilot (nl.trustpilot.com/review/moneybird.nl) | 17 | Profiel: **259 reviews, TrustScore 2,2**, "99 reviews in de afgelopen 12 maanden". Gefilterde pagina 2–4★ (1 pagina) via web-fetch + 19 (vooral Engelstalige) reviews via `automation-lab/trustpilot` |
| **Totaal** | **61** | |

- **Verdeling** (script over `data/moneybird.csv`): 1 ster 16 · midden 38 · positief 7
- **Periode**: 2022-05 t/m 2026-11; **47 van 61 rijen van na nov 2024**. De 14 oudere rijen zijn app-reviews over offertes/facturen in de app (gemarkeerd met datum in de citaten).
- **Kwaliteitsnoten**:
  - **Bewuste selectie** op de prioriteit-2-thema's; de positieve groep is ondervertegenwoordigd. De app-stores zijn voor Moneybird duidelijk positiever dan Trustpilot (veel korte 5★ "top"-reviews die niet zijn opgenomen).
  - **Trustpilot wordt gedomineerd door de pakketwijziging van zomer 2026** (vervallen gratis pakket, bankkoppeling pas vanaf Groei, Ponto-verplichting) en door AI-only support ("Vink"). Dat zijn deels boekhoud-/prijsonderwerpen; alleen de koppelings- en lock-in-aspecten zijn meegenomen.
  - **Geen vakbedrijven herkenbaar.** Eén Google Play-reviewer (3★, 2026-07) vraagt om calculatie/marges en een klant-intakelink – dat past bij een vakman, maar de branche wordt niet genoemd.
  - **Niet opgehaald**: Capterra (WebSearch toont 1 review), G2 (14 reviews, laag volume, niet opgehaald om credits te sparen). Feedback Company (gelinkt vanaf moneybird.nl) niet opgehaald.

## Wat gebruikers goed vinden (de lat)

1. **Offerte → factuur is eenvoudig**: "Makkelijk offertes maken en bij goedkeuring eenvoudig om te zetten naar factuur. Werkt perfect." (Google Play, 5★, 2023-01-26; oud). "Offertes, facturen, terugkerende facturen, incasseren… werkt allemaal erg goed!" (Google Play, 5★, 2024-10-03)
2. **Facturen vanaf de telefoon versturen**, als het werkt: "Facturen inboeken en versturen kan eenvoudig via de app" (App Store, 5★, 2025-02-12).
3. **Web-product is sterk; de app volgt**: "The actual MoneyBird system (via website) is awesome full of features." (App Store, 3★, 2024-12-11). "Zeer intuïtief boekhoudpakket met uitgebreide mogelijkheden" (Trustpilot, 4★, 2026-10-11).
4. **API**: "fully automated everything using their great api." (Trustpilot, 5★, 2025-03-03)

## Top 5 pijnpunten

| # | thema | freq. (1★/midden) | ernst | toelichting |
|---|---|---|---|---|
| 1 | mobiel (app beperkt t.o.v. web) | 35 (12/23) | hoog | app is "kijk-en-scan"-app; offertes/facturen afmaken vaak alleen op de pc |
| 2 | bugs/stabiliteit na updates | 22 (9/13) | hoog | vastlopen bij factuurregels, login/passkey-problemen, uploads die mislukken |
| 3 | facturatie in de app | 15 (4/11) | middel–hoog | factuur aanpassen/scrollen, datum per regel, pdf downloaden |
| 4 | prijs / lock-in rond pakketwijziging | 12 prijs, 6 lock-in | middel | bankkoppeling achter duurder pakket; oude facturen niet meer in te zien |
| 5 | offerte-functionaliteit | 9 (1/8) | middel | één prijstabel, geen opdrachtbevestiging, offertes kwijt in de app |

Ook: koppelingen (bank/Ponto/Knab) 7×, support (alleen AI/schriftelijk) 7×, tablet-app ontbreekt 3×.

**1. Mobiel**
- "De web werkt dus beter dan de app…" (App Store, 1★, 2025-10-17)
- "Ergens kan ik begrijpen dat het vooral is gericht op 'de ondernemer onderweg'… App: 2/5; website: 4/5" (Google Play, 3★, 2024-07-08)
- "The app is restricted to doing the most basic of tasks - it's only useful for scanning receipts." (Trustpilot, 1★, 2024-11-21)

**2. Bugs/stabiliteit**
- "Bug na bug, vastlopen op vastlopen, zeer irritant." (App Store, 3★, 2026-10-17)
- "loopt de app vaak vast als ik bijv een regel toevoeg en daarna nog 1" (App Store, 4★, 2026-02-12)
- "Every weekly release brings new random failures" (Trustpilot, 2★, 2026-10-05; lange review, niet in CSV-tekst)

**3. Facturatie in de app**
- "aanpassen van een factuur op de mobiele versie niet meer te doen." (App Store, 1★, 2026-11-04)
- "elke keer wanneer ik een factuur wilt maken loopt het vast" (App Store, 1★, 2025-10-13)
- "datums per dag zou kunnen invoeren, dit werkt nog altijd alleen maar met gebruik op de pc of laptop." (Google Play, 4★, 2024-04-11)

**4. Prijs/lock-in en koppelingen**
- "Een automatische bankkoppeling is tegenwoordig een basisfunctionaliteit… geen premiumfunctie." (Trustpilot, 2★, 2026-07-31)
- "nu kan ik niet meer in mijn account om oude facturen in te zien." (App Store, 2★, 2026-10-15)

**5. Offerte**
- "veel functies werken niet… downloaden PDF, offertes opzoeken… Dit is erg frustrerend als je zaken wilt doen met potentiële klanten." (App Store, 1★, 2026-06-10)
- "er maar één prijstabel mogelijk is" (App Store, 4★, 2024-06-06; oud)
- "jammer dat er geen opdrachtbevestiging verstuurd kan worden." (App Store, 4★, 2024-10-04)

## "Wat net mist" (uit middenreviews)

- **De offerte afmaken op locatie.** Middenreviewers willen in de app een bestaande offerte aanpassen en factureren, korting/datum per regel zetten en de klant laten tekenen op een tablet. "Ik heb een iPad gekocht om klanten makkelijker te kunnen laten tekenen… dan is de app niet ingericht" (3★, 2023-12-23; oud). Geen iPad-app (3×).
- **Calculatie en marges bij de offerte** en een **link waarmee de klant zelf zijn gegevens invult** (Google Play, 3★, 2026-07-02) – precies de intake- en calculatiestap vóór de offerte.
- **Opdrachtbevestiging** als apart document na akkoord (4★, 2024-10).
- **Onthouden van filters/status in de app** (factuuroverzicht moet steeds opnieuw gefilterd).
- **Betrouwbare koppelingen**: bankkoppeling via Ponto/Knab hapert en zit nu achter het Groei-pakket; middenreviewers accepteren het product maar niet dat een "basisfunctie" duurder wordt.

## Kansen voor ons CRM

- **Mobiele offerte als volwaardige flow** (aanmaken, regels/korting aanpassen, laten tekenen op telefoon of tablet, versturen) – de app van een van de populairste NL-facturatiepakketten faalt hier juist. Dit is de lat om over te springen, niet om te halen.
- **Koppelen in plaats van vervangen**: Moneybird heeft een gewaardeerde API en is populair bij kleine ondernemers. Een betrouwbare één-klik-doorzet van geaccepteerde offerte → Moneybird-factuur (incl. klantgegevens) is waarschijnlijk waardevoller dan eigen facturatie. Let op: koppelingen moeten stabiel zijn; haperende koppelingen zijn een terugkerende ergernis.
- **Klant-intakelink** (klant vult zelf adres/contact in) sluit aan op lead-opvang en klantdossier per adres – één middenreviewer vraagt hier letterlijk om.
- **Calculatie/marge in de offerte** en **opdrachtbevestiging** als standaardstap na akkoord.
- **Stabiliteit en menselijke support als belofte**: Moneybird verliest vertrouwen door wekelijkse releases met regressies en AI-only support. Voor een vakman die op de steiger een offerte wil versturen is "het werkt altijd" een verkoopargument.
- **Lead-opvang, WhatsApp, nazorg/onderhoud**: geen data in deze reviews.
