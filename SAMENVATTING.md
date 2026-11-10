# SAMENVATTING – review-analyse software voor technische vakbedrijven (NL)

*Peildatum: 10 november 2026. Basis: 26 tools (20 prioriteit 1, 6 prioriteit 2), 981 reviewrijen. Per tool staan de details in `analyse/<tool>.md` en de ruwe reviews in `data/<tool>.csv`.*

**In één alinea.** De bestaande tools worden vooral beoordeeld op één ding: werkt de app in het veld en blijft de data betrouwbaar? De meest genoemde klachten over software zijn bugs en dataverlies na updates, een mobiele app die achterloopt op de webversie, eenzijdige prijsverhogingen en het gevoel vast te zitten. Over **lead-opvang, offerte-opvolging, WhatsApp en nazorg** wordt in de reviews bijna niet geklaagd. Dat komt doordat bijna geen enkele tool deze processen bedient, zodat er ook niets te klagen valt. Het bewijs dat hier een gat zit, komt van de leadplatforms. Daar betalen vakmannen €3–75 per contact. Ze krijgen leads die ze met 3–10 concurrenten delen en die binnen een uur alweer weg zijn. En ze hebben geen instrument om snel op te volgen of om te meten welke bron wat oplevert. Een CRM dat wint op **snelheid van eerste reactie + opvolging + eigen klantbezit**, zonder het werkbon-/ERP-terrein na te bouwen, heeft hier ruimte.

---

## 1. Databasis en kwaliteit in één oogopslag

| Tool | Reviews in CSV | 1★ / midden / positief | Sinds nov 2024 | Kwaliteit |
|---|---:|---|---:|---|
| OutSmart | 100 | 48 / 33 / 19 | 45 | **Goed**; Trustpilot-cluster rond prijswijziging nov 2024 |
| Simple-Simon | 65 | 9 / 10 / 46 | 12 | Matig: grotendeels oud en positief gekleurd ("recensies worden min of meer gedwongen") |
| Gripp | 41 | 17 / 18 / 6 | 20 | Redelijk; doelgroep vooral bureaus, Capterra-reviews komen uit één campagne in 2021 |
| Workmate | 19 | 0 / 3 / 16 | 12 | Dun; alleen Google-reviews, die waarschijnlijk zijn opgevraagd |
| Spotmaster | 2 | – | 2 | **Onbruikbaar**; maatwerkleverancier |
| Tradecount | 0 | – | – | **Niet gevonden**; de naam klopt mogelijk niet |
| WeFact | 97 | 27 / 52 / 18 | 82 | Goed, maar 34 rijen zijn gedwongen ex-FactuurSturen-migranten; maar 3 reviewers zijn herkenbaar vakbedrijf |
| BouwBit | 0 | – | – | **Geen softwarepakket** (IT-dienstverlener) |
| Exact Bouw7 | 69 | 18 / 17 / 34 | 12 | Redelijk; het positieve beeld is oud (2015–2019), het recente beeld negatief |
| Syntess | 3 | – | 0 | Onbruikbaar |
| KRAAN | 1 | – | 0 | Onbruikbaar |
| Admicom | 0 | – | – | Geen publieke reviews |
| Sollit (ex-2Solar) | 13 | 5 / 4 / 4 | 3 | Zeer dun |
| Solar Monkey | 0 | – | – | Geen gebruikersreviews gevonden |
| OpusFlow | 4 | 0 / 2 / 2 | 2 | Zeer dun; G2-gemiddelde 4,4 (7 reviews) zonder leesbare teksten |
| Teamleader Focus | 74 | 24 / 34 / 16 | 27 | Goed voor de app en prijs; maar 4 reviewers zijn aantoonbaar bouw/installatie |
| Werkspot (vakman) | 129 (118 vakman) | 96 / 29 / 1 | 110 | **Goed**; Trustpilot gefilterd op 1–3★ (negatieve bias) |
| Solvari (vakman) | 34 (25 vakman) | alle vakman-rijen 1★ | 14 | Dun en grotendeels 2023–2024 |
| Trustoo (vakman) | 54 (47 vakman) | alle vakman-rijen 1★ | 54 | Redelijk en recent, maar eenzijdig: geen positieve vakman-reviews gevonden |
| Zoofy (vakman) | 38 (35 vakman) | 22 / 9 / 4 (vakman) | 22 | Redelijk; veel app-reviews gaan alleen over aanmelden |
| *Prioriteit 2 (alleen offerte/facturatie, koppelingen, app)* | | | | |
| Moneybird | 61 | 16 / 38 / 7 | 47 | Redelijk; geen reviewer herkenbaar als vakbedrijf |
| e-Boekhouden.nl | 40 | 6 / 27 / 7 | 25 | Dun; App Store-reviews grotendeels oud |
| SnelStart | 49 | 13 / 34 / 2 | 36 | Redelijk; 2 reviewers herkenbaar vakbedrijf |
| Exact Online | 74 | 46 / 28 / 0 | 67 | Redelijk; 3 reviewers bouw/installatie |
| HubSpot | 5 | 0 / 4 / 0 (+1 forumvraag) | 5 | Indicatief; alleen VS-bouw/facilities (Capterra.com) |
| Pipedrive | 9 | 1 / 7 / 1 | 8 | Indicatief; alleen VS-bouw/renewables (Capterra.com) |

*De groepsindeling in deze tabel is achteraf over alle CSV's herberekend met één regel: 1★ / 2–3★ of 4–5★ mét klachtcode = midden / 4–5★ zonder klacht = positief. Daardoor wijkt hij soms 1–2 rijen af van de per-tool-analyse.*

**Belangrijkste kanttekeningen**
1. **Selectie-bias.** De middengroep en de 1★-groep zijn bewust oververtegenwoordigd. De opdracht was immers de middenreviews te zoeken, en bij WeFact, Teamleader, Werkspot en Zoofy zijn de Trustpilot-reviews gefilterd op 1–3★. De tellingen zeggen dus *welke* klachten vaak terugkomen, niet hoe tevreden de markt gemiddeld is.
2. **Grote ERP's hebben geen publieke reviews.** Syntess, KRAAN en Admicom worden verkocht met demo en implementatietraject; kopers schrijven geen app-store-reviews. Wat deze tools goed of slecht doen, valt alleen met interviews vast te stellen.
3. **Weinig vakbedrijven herkenbaar.** Bij WeFact, Teamleader en Gripp is het merendeel van de reviewers generiek mkb. Voor de werkbon-tools (OutSmart, Simple-Simon, Bouw7, Sollit) mag je aannemen dat de app-reviewers vakmensen in het veld zijn, want die apps zijn alleen voor hen bedoeld.
4. **Bronnen die vanuit deze omgeving niet lukten.**
   - G2: nergens op te halen (time-outs en blokkades).
   - Capterra.com: deels time-outs.
   - LinkedIn en YouTube-comments: niet systematisch doorzocht.
   - Tweakers en Reddit: vrijwel niets relevants gevonden.
   - Kassa: geen vakman-item gevonden.

---

## 2. Tabel: tool × top-pijnpunten

Het getal is het aantal reviews dat het thema noemt; een review kan meerdere thema's hebben. Een streepje betekent dat het thema niet in de top van die tool staat of dat er te weinig data is.

| Tool | #1 | #2 | #3 | #4 | #5 |
|---|---|---|---|---|---|
| OutSmart | bugs/dataverlies na updates (50) | mobiel, vooral Android (18) | werkbon/uren onbetrouwbaar (17) | prijs ×3–4 in 2024 (13) | support (11), lock-in (8) |
| Simple-Simon | mobiel (7) | bugs (6) | werkbon-invoer omslachtig (5) | gebruiksgemak (4) | support alleen per mail (3) |
| Gripp | prijsverhoging na Exact-overname (16) | support / AI-bot (11) | lock-in: export kost €169 (5) | mobiel (5) | bugs / stilstand (4) |
| Workmate | implementatie vraagt finetuning (2) | aanpassen alleen via maatwerk (1) | – | – | – |
| WeFact | gebruiksgemak (26) | onboarding/migratie (21) | bugs: betalingen kwijt (21) | mobiel = alleen kijken (20) | support (16), prijs/Plus (13) |
| Exact Bouw7 | bugs/storingen (24) | mobiel: steeds opnieuw inloggen (17) | uren/bonnen op locatie (5) | gebruiksgemak (5) | koppeling boekhouding, rapportage (1–2) |
| Sollit | mobiel (8) | bugs na updates (6) | planning-UI (2) | offerte niet aanpasbaar in app (1) | – |
| Teamleader Focus | mobiel (29) | bugs (19) | prijs: min. 2 gebruikers, verhogingen (18) | support (14) | lock-in: jaarcontract, deurwaarder (13) |
| Werkspot | leadkosten (93) | leadkwaliteit (58) | support/restitutie (42) | lead-concurrentie 5–10+ (20) | bugs (13) |
| Solvari | leadkosten (21) | reclamatie/support (13) | leadkwaliteit (11) | lock-in: 1–3-jaarscontract (11) | "exclusief" blijkt gedeeld (4) |
| Trustoo | leadkosten (37) | leadkwaliteit (29) | support: wie reclameert wordt minder zichtbaar (23) | lead-concurrentie (11) | lock-in: pauze/opzeggen werkt niet (7) |
| Zoofy | support (13) | leadkosten + tarief (19) | onboarding/ID-check (10) | bugs (9) | uitbetaling te laat (7) |
| Spotmaster, Tradecount, BouwBit, Syntess, KRAAN, Admicom, Solar Monkey, OpusFlow | te weinig data | | | | |
| *Prioriteit 2* | | | | | |
| Moneybird | mobiel: app beperkt t.o.v. web (35) | bugs na updates (22) | facturatie in app (15) | prijs/pakketwijziging 2026 (12), lock-in (6) | offerte: één prijstabel, geen opdrachtbevestiging (9) |
| e-Boekhouden.nl | mobiel: fractie van de website (20) | gebruiksgemak/verouderd (14) | facturatie-details (13) | bugs (6) | koppelingen (4) |
| SnelStart | mobiel, vooral inloggen (28) | bugs (23) | facturatie (12) | support (8) | prijs: API-toegang via duurder pakket (7), koppelingen (6) |
| Exact Online | mobiel (68) | bugs/regressies na updates (53) | facturatie: uploaden/delen/Peppol (27) | support (9) | gebruiksgemak (9) |
| HubSpot | prijs bij groei (3) | gebruiksgemak (2) | onboarding: geen sjabloon voor aannemers (1) | rapportage in hogere tiers (1) | – |
| Pipedrive | gebruiksgemak (3) | geen prijslijst/voorraad in offerte (1) | geen telefonie (1) | onvolledige webformulieren (1) | – |

---

## 3. De 10 meest voorkomende frustraties in de markt

Gerangschikt op **frequentie × ernst**.
- **Frequentie** = aantal reviews met dit thema, over alle tools (vakman-rijen, zonder consumenten).
- **Ernst**:
  - 3 = kost direct geld, data of een klant;
  - 2 = dagelijkse frictie in het werk;
  - 1 = ergernis.

Software en leadplatforms zijn samengenomen, omdat het om dezelfde vakman gaat.

| # | Frustratie | Freq. | Ernst | Score | Tools | Typerend citaat |
|---|---|---:|---:|---:|---|---|
| 1 | **Betalen voor leads die niets opleveren** (kosten per contact) | 161 | 3 | 483 | Werkspot, Trustoo, Solvari, Zoofy | "moet direct lead kosten betalen (vaak tussen €10 en €40) … Reageert de consument niet? … 99% van de tijd word je restitutie aanvraag geannuleerd" (Werkspot, Trustpilot, 2026-10-30) |
| 2 | **Bugs, dataverlies, storingen na updates** | 154 | 3 | 462 | 9 van de 9 softwaretools met data | "na een zoveelste update er weer oude problemen … Foto's, certificaten, documenten, emailadressen van klanten, serienummers worden niet meer opgeslagen" (OutSmart, Google Play, 2022-04-12) |
| 3 | **Support onbereikbaar of afwijzend** (incl. restitutie) | 148 | 2 | 296 | alle grote tools | "Telefoonnummer op hun site afgesloten, Chat 3 uur wachten." (Trustoo, Trustpilot, 2025-11-25) |
| 4 | **Leadkwaliteit**: onbereikbaar, nep, alleen prijs opvragen | 99 | 3 | 297 | leadplatforms | "27 leads … waarvan er 20 niet eens antwoorde op mijn eerste bericht, terwijl ik er altijd binnen 5 minuten bij was" (Trustoo, Trustpilot, 2026-01-31) |
| 5 | **Mobiele app loopt achter op het platform**: uitloggen, geen offline, alleen kijken | 118 | 2 | 236 | 9 tools | "De app reflecteert niet de rest van het platform." (Teamleader, App Store BE, 2023-10-06) |
| 6 | **Eenzijdige prijsverhoging / prijsmodel** | 70 | 2 | 140 | OutSmart, Gripp, Teamleader, WeFact, Zoofy | "Na de overname door Exact zijn de prijsstijgingen de pan uit gerezen!" (Gripp, Trustpilot, 2025-06-27) |
| 7 | **Lock-in**: jaarcontract, geen volledige export, deurwaarder | 65 | 2 | 130 | Gripp, OutSmart, Teamleader, WeFact, Solvari, Trustoo | "Dit voelt als een gijzeling … dit kost ook €169,- als je door hen een export wil laten maken." (Gripp, Trustpilot, 2025-01-09) |
| 8 | **Lead gedeeld met 3–10 concurrenten**: wie het eerst reageert, wint | 35 | 3 | 105 | Werkspot, Trustoo, Solvari | "als je een aanvraag krijgt per email en whatsapp en gelijk opent hebben 3 andere personen al gereageerd." (Trustoo, Trustpilot, 2025-11-25) |
| 9 | **Gebruiksgemak**: te veel klikken, slecht zoeken | 71 | 1–2 | ~105 | 9 tools | "Slechte Zoek functie op adres totaal niet handig bij meerdere klanten" (WeFact, Google Play, 2022-08-03) |
| 10 | **Onboarding/migratie zwaar**, maandenlang "finetunen" | 56 | 2 | 112 | 8 tools + Zoofy | "Het is wel wat finetunen wanneer het in bedrijf is" (Workmate, Google Maps, 2025-04-15) |

Net buiten de top 10: werkbon/uren onbetrouwbaar (34 × 2) en facturatie/boekhoudkoppeling "net niet" (32 × 2).

**Alleen software, zonder leadplatforms** (488 rijen):
1. bugs 132
2. mobiel 107
3. gebruiksgemak 66
4. prijs 61
5. support 57
6. onboarding 42
7. lock-in 36
8. werkbon 34
9. facturatie 31
10. planning 21

**Prioriteit 2 bevestigt het beeld.** In de 278 rijen over boekhoudpakketten en generieke CRM's staat **mobiel** bij alle vier de NL-boekhoudpakketten op #1 (Exact Online 68, Moneybird 35, SnelStart 28, e-Boekhouden 20), gevolgd door bugs na updates. Dezelfde top-2 als bij de werkbon-tools.

**De lat** (wat gebruikers het vaakst expliciet waarderen in de software-reviews):
- gebruiksgemak, juist voor monteurs (60×)
- bereikbare, persoonlijke support (58×)
- snel en mooi offertes maken (21×)
- een soepele inrichting (16×)
- koppelingen met boekhouding (15 + 8×)
- een app die gewoon werkt (15×)

---

## 4. Gaten die géén enkele tool goed oplost

De belangrijkste bevinding is een *afwezigheid*: in 488 software-reviews komen lead-opvang, offerte-opvolging, WhatsApp en nazorg samen nog geen 20 keer voor. Dat is geen bewijs dat niemand ze nodig heeft. Het laat wel zien dat de tools die deze vakmensen gebruiken deze processen niet bedienen. De klachten over de leadplatforms laten zien dat de pijn er wél is.

**4.1 Lead-opvang: snelheid en meerdere kanalen**
- **Geen tool bundelt aanvragen** uit WhatsApp, mail, website en leadplatforms. Eén OutSmart-gebruiker heeft zelf het hele proces "van aanvragen op onze website tot aan de facturatie geautomatiseerd" (SoftwareWatcher, z.d.). Dat is maatwerk en geen standaardfunctie.
- **Op de leadplatforms is snelheid de enige winfactor**: "hebben 3 andere personen al gereageerd" (Trustoo, 2025-11-25). Ook: "leads die binnen 1 uur (!) een schrijven stuurt dat ze al een ander hebben gevonden" (Trustoo, 2026-04-29). Vakmannen hebben daar geen instrument voor.
- **Geen kosten/opbrengst per leadbron.** "Over maart hebben wij een openstaande rekening van € 1.244. Verwachte omzet van de leads is circa € 925." (Trustoo, dienstverlener, 2026-03-28). Het rekenwerk doet de vakman nu zelf.

**4.2 Offerte-opvolging**
- **Weinig tools tonen of de klant de offerte heeft bekeken.** Teamleader doet dit en het wordt expliciet gewaardeerd: "kan ik precies zien hoe vaak mijn klanten de offerte hebben bekeken, wat me helpt om op het juiste moment te volgen" (Trustpilot, 2024-07-26). Bij WeFact zitten opvolging en "geopend" alleen in het duurdere Plus-pakket.
- **Een gespreksverslag met vervolgactie op de mobiel ontbreekt.** "De app mist dat als je een verkoopgesprek hebt gehad dat je dan eenvoudig een gespreksverslag kunt maken met vervolgactie. Dit is essentieel voor buitendienst" (Teamleader, App Store NL, 2023-09-15).
- **Offertes voor maatwerk passen niet in generieke CRM's.** "Je werkt letterlijk drie keer aan hetzelfde project om één offerte klaar te krijgen" (Teamleader, plaatser BE, 2026-08-10). Ook gemist: de offerte ter plekke in de app aanpassen (Sollit, 2021) en offertes vanaf de telefoon versturen (WeFact, 2020).

**4.3 WhatsApp en klantcommunicatie**
- **Geen enkele tool heeft een werkende WhatsApp-integratie** in de reviews. Teamleader had alleen een link en die verdween: "Met de oude app kon ik nog linkjes naar whatsapp openen… Sinds de nieuwe app kan dat niet" (Google Play, 2024-05-14).
- **Bij Bouw7 wordt WhatsApp zelfs intern gevraagd**: "Nog beter als er een WhatsApp komt als je week uren niet kompleet zijn" (Google Play, 2023-06-14).
- **Er is geen controle of een bericht aankomt**: "stuur ik een factuur weg met een fout e mail adres … krijg ook geen melding dat de factuur uiteindelijk niet verstuurd is" (WeFact, 2025-12-14). En: "soms worden de werkbonnen niet verstuurd via de email" (OutSmart, Google Play, 2025-10-16).
- **De leadplatforms bezitten het klantcontact.** Wordt een account geblokkeerd, dan ben je ook je reviews en contacten kwijt (Werkspot-analyse).

**4.4 Klantdossier per adres en objecthistorie**
- **Gewaardeerd waar het bestaat**: foto's "gelijk bij de betreffende klant in de klantenmap" (Workmate, 2023-06-20), "automatisch een dossier opbouwen" en "geschiedenis gemakkelijk te bekijken voor de monteurs onderweg" (Simple-Simon, 2022/2023).
- **Mis waar het faalt**:
  - "niet kunt zien wat de vorige problemen waren met de machine en wat er is gedaan" (OutSmart, App Store, 2022-10-22).
  - Zoeken op adres werkt slecht (WeFact, 2022).
  - Eén contactpersoon die bij meerdere klanten hoort staat tot tien keer in het systeem (Gripp, 2026-10-10).
  - Interne notities of bijlagen die de klant niet ziet ontbreken (WeFact, 2026-07-29).

**4.5 Nazorg en onderhoud**
- **Alleen de werkbon-/ERP-tools doen dit**: Simple-Simon met periodiek onderhoud, OpusFlow met checklists voor ketelonderhoud, Workmate met preventief onderhoud.
- **Het wordt sterk gewaardeerd, maar mist bij de lichtere tools**: "kijken uit naar de jaarplanning die gaat komen" (Simple-Simon, 2022). Gripp heeft geen terugkerende opdrachten (2021).
- **Niemand koppelt onderhoud aan herhaalomzet.** Er is geen voorbeeld van een automatische onderhoudsherinnering of reviewverzoek naar de klant, en evenmin van een upsell vanuit het dossier. Dit gat is afgeleid uit afwezigheid; geen reviewer vraagt er letterlijk om.

---

## 5. Wat vakmannen over leadplatforms zeggen

Gebaseerd op 225 vakman-reviews: Werkspot 118, Trustoo 47, Zoofy 35, Solvari 25.

**De kern: vakmannen zijn niet tegen betalen voor werk, wel tegen betalen voor contact.** "Als ik 150 zou moeten betalen per klant, geen enkel probleem" (Trustoo, 2026-01-31).

| Aspect | Wat vakmannen melden |
|---|---|
| **Kosten per lead** | Werkspot €3–75 per lead (FAQ, aug 2026); reviewers zien de gemiddelde prijs stijgen van "rond de €20" naar "€40" (Trustpilot, 2026-07-05). Trustoo €12,50–40 per aanvraag plus sinds eind 2025 een Premium-bijdrage. Solvari €25–30 per lead of campagnes van €355–2.200 per maand met contracten van 1–3 jaar. Zoofy werkt met een abonnement plus marge: "de klant €150+ betaalt, en jij … nog geen €60-€70" (Trustpilot, 2026-03-12). |
| **Kwaliteit** | Klanten onbereikbaar of het nummer klopt niet; aanvragen "uitsluitend bedoeld om een indicatie van de kosten te krijgen" (Werkspot, 2026-08-25); "Meer dan 50% vraagt hun met rust te laten" (Solvari, warmtepompinstallateur, 2025-12-26); filters en subcategorieën te grof (Trustoo). |
| **Concurrentie** | 3–5 bedrijven per lead (Trustoo), 5–10+ (Werkspot), "exclusief" blijkt aan 7–10 bedrijven verkocht (Solvari). "De leads worden met 5 bedrijven gedeeld je moet vechten om mee te kunnen eten" (Trustoo, 2025-11-18). |
| **Opvolging** | Snelheid beslist; klanten zeggen "al binnen 4 uur dat ze iemand hebben gevonden" (Trustoo, 2025-11-18) of melden "binnen 1 uur" dat ze al een ander hebben (Trustoo, 2026-04-29). De consument weet niet dat reageren de vakman geld kost (Werkspot, 2026-08-05). Het Trustoo-dashboard is geen werkinstrument. |
| **Restitutie en support** | Restitutie standaard afgewezen ("99% … geannuleerd"), een reclamatielimiet die "meteen vol is" (Solvari), wie reclameert wordt minder zichtbaar (Trustoo), en snel incasso. |
| **Afhankelijkheid** | Reviews en klantcontacten zijn van het platform. Bij Zoofy wordt de uitbetaling (na ca. 29 dagen) ingehouden bij een klacht. |

**Implicatie.** Een CRM hoeft niet te concurreren met de leadplatforms. Het moet de vakman helpen (a) betaalde leads sneller en beter op te volgen, (b) te meten welk platform rendeert, en (c) stap voor stap eigen herhaalklanten en eigen reviews op te bouwen. Solvari biedt zelf al een eenvoudig CRM aan (Essential-pakket, ±€49 per maand, niet geverifieerd); het onderscheid zit dus in **platform-onafhankelijkheid**.

---

## 5b. Prioriteit 2: boekhouding en generieke CRM's (offerte, koppelingen, mobiel)

- **Boekhoudpakketten zijn geen offertetool voor vakmensen.** "voor installatiebedrijven het meest onvriendelijke boekhoud programma wat er is… Als installateur maak ik hier ook mn offertes etc in maar dat werkt maar voor de helft." (Exact Online, App Store, 2026-11-02, installateur). Bij Moneybird is het hetzelfde: één prijstabel, geen opdrachtbevestiging en geen app die werkt op de iPad om de klant te laten tekenen ("heb een iPad gekocht om klanten makkelijker te kunnen laten tekenen… dan is de app niet ingericht om op een iPad", Moneybird).
- **Zoeken op adres ontbreekt ook hier.** "Enkel op naam zoeken in plaats van ook op adres of woonplaats." (SnelStart, App Store, 2026-04-01). Dit bevestigt het klantdossier per adres (§4.4).
- **Koppelen wordt duurder gemaakt.** SnelStart: API-toegang betekent "verplicht upgraden van 22 naar 54 euro per maand… en je na afloop ook nog eens 250 euro certificeringskosten" (reviewer). Bij Moneybird zit de bankkoppeling sinds de pakketwijziging van 2026 pas in het Groei-pakket (€29, volgens de per-tool-analyse). Een koppeling via UBL/Peppol-export plus de standaard-API's van Moneybird, e-Boekhouden en Exact verlaagt de drempel voor de klant.
- **WhatsApp wordt ook hier gevraagd, maar is nergens ingebouwd.** "…koppeling maken naar een SMS./ whatsapp sturen bij contact ?" (e-Boekhouden, Google Play, oud).
- **HubSpot en Pipedrive (VS-bouw, dunne data).** Pipedrive wordt gewaardeerd om de visuele pipeline per klusfase: "keeps our team accountable, and ensures no follow-ups are missed" (Capterra.com). Het is ook goedkoper dan het branchepakket AccuLynx. HubSpot "seems built only for big companies" (Capterra.com). Dit laat zien dat een **simpele pipeline + automatische opvolging** het deel van een generiek CRM is dat aannemers echt gebruiken. Ze missen er wel prijslijsten, vakspecifieke sjablonen en telefonie in.

## 6. Feature- en positioneringsaanbevelingen

Elke aanbeveling is onderbouwd met bewijs uit de reviews. De volgorde is een voorstel voor prioriteit.

### Positionering
**"Van aanvraag tot terugkerende klant – voor vakbedrijven die geen ERP willen."** Het CRM zit vóór en ná de werkbon. Daarbij twee keuzes:
- **Bouw de werkbon/planning niet na.** Het grootste deel van de klachten over werkbon-tools gaat over hun kern: stabiliteit, sync en de app in het veld. Dat terrein is bezet en duur om goed te doen. Koppel liever met OutSmart, Simple-Simon, Bouw7 en de boekhoudpakketten.
- **Beloof en meet betrouwbaarheid, prijsstabiliteit en vrije export.** Dat zijn de drie emoties achter de meeste 1★-reviews: bugs (132), prijs (61) en lock-in (36) in software.

### Features

| # | Feature | Waarom (bewijs) |
|---|---|---|
| 1 | **Eén lead-inbox**: Werkspot/Trustoo/Solvari-mails, websiteformulier, WhatsApp Business en telefoon, automatisch omgezet naar een lead met adres | Snelheid beslist (lead-concurrentie 35×, "3 andere personen al gereageerd"); geen enkele tool doet dit standaard |
| 2 | **Reactie binnen minuten**: push naar de mobiel, één tik voor een WhatsApp- of sms-sjabloon, belknop die het gesprek automatisch logt | Klant "binnen 1 uur" / "binnen 4 uur" weg (Trustoo); Teamleader-app: "niet geregistreerd dat je gebeld hebt", "geen push notificaties" |
| 3 | **Kwalificatievragen en foto's opvragen via WhatsApp** voordat je rijdt | "aanvragen te vaag om een prijs te kunnen geven" (Werkspot); "betere omschrijving van de klus" (Zoofy) |
| 4 | **Leadbron-ROI**: kosten per platform invoeren of importeren tegenover offertes en omzet, plus een restitutiedossier (belpogingen met tijdstempel als bewijs) | "openstaande rekening € 1.244 … verwachte omzet € 925" (Trustoo); restitutie "99% geannuleerd" (Werkspot) |
| 5 | **Offerte-opvolging standaard, niet als duurdere add-on**: "geopend"-melding, automatische herinneringsreeks (mail + WhatsApp), digitaal tekenen met 1 klik | Expliciet gewaardeerd bij Teamleader ("hoe vaak … bekeken"; "met 1 klik bevestigen"); bij WeFact alleen in Plus (+€10 per maand) |
| 6 | **Snelle offerte voor maatwerk** op mobiel en desktop, met eigen calculatieblokken per vak (m², strekkende meter, stelpost) en ter plekke aanpasbaar | "drie keer aan hetzelfde project om één offerte" (Teamleader, plaatser); "offerte aanpassen in de app" (Sollit); "vanaf een iPhone versturen" (WeFact) |
| 7 | **Klantdossier per adres** (niet per persoon): foto's, offertes, werkbonnen uit de gekoppelde tool, interne notities en bijlagen, meerdere contactpersonen per adres | Gewaardeerd bij Workmate/Simple-Simon; gemist bij OutSmart (historie), WeFact (zoeken op adres, interne notities) en Gripp (dubbele contacten) |
| 8 | **Nazorg-automaat**: onderhouds- en keuringsherinneringen per object (cv-ketel, warmtepomp, dak, schilderwerk), reviewverzoek na oplevering, jaarlijkse check-in via WhatsApp | Onderhoudsplanning wordt gewaardeerd waar het bestaat (Simple-Simon, OpusFlow, Workmate) en gemist waar het ontbreekt (jaarplanning, terugkerende opdrachten); eigen reviews verminderen de afhankelijkheid van platforms |
| 9 | **Bezorgcontrole**: bevestiging dat een mail of WhatsApp is afgeleverd, en een melding bij een fout adres | WeFact 2025-12-14; OutSmart 2025-10-16 |
| 10 | **Mobiel-eerst en "blijft ingelogd"**, met offline wachtrij | Mobiel is #2 in software (107×); uitloggen is een terugkerende klacht bij Bouw7 en Teamleader |
| 11 | **Koppelingen die wél volledig zijn** (Moneybird, e-Boekhouden, SnelStart, Exact; werkbon-tools) en een openbare API; zelf **geen boekhouding bouwen**, maar offerte → factuur doorzetten (API of UBL/Peppol) | "Koppeling … houtje touwtje werk" (Bouw7); de Exact-koppeling werkt "net niet" (OutSmart); koppelingen zijn een positief punt bij Teamleader en WeFact; SnelStart-API kost de klant een upgrade naar €54 per maand + €250 certificering |
| 12 | **Eerlijk prijsmodel**: per bedrijf of gebruiker zonder minimum van 2, maandelijks opzegbaar, gratis volledige export (CSV/Excel + bijlagen), prijsgarantie | Prijs (61) en lock-in (36) in software; "€169 voor een export" (Gripp); Teamleader-minimum van 2 gebruikers; jaarcontract met deurwaarder |
| 13 | **Inrichting in een dag**: sjablonen per vak (dakdekker, installateur, schilder), import uit Excel, WeFact, Teamleader en Gripp | Onboarding 42×; "drie keer finetunen" (Workmate); "meedenken en adviseren over hoe we het beste kunnen inrichten" (Teamleader) |
| 14 | **Persoonlijke, telefonisch bereikbare support** als verkoopargument | Support is de nummer-2-waardering (58×) én een top-klacht (57× in software, 148× in totaal) |

### Wat we níét moeten doen (lessen uit de reviews)
- **Geen grote updates zonder terugvaloptie.** Dataverlies na updates is de topklacht bij OutSmart, Bouw7 en Sollit.
- **Geen functies van het basispakket naar duurdere pakketten verschuiven.** Dat zie je terug in de 1★-reviews over WeFact en Gripp.
- **Geen AI-chatbot in plaats van mensen bij de support** (Gripp).
- **Reviews niet "afdwingen"** zoals bij Simple-Simon: dat ondermijnt de geloofwaardigheid.

---

## 7. Bronnenlijst en kwaliteitsnoot per tool

Alle reviews zijn op 10 november 2026 opgehaald via Apify-scrapers (Google Play, App Store, Trustpilot, Google Maps) en Apify web-fetch (Capterra, Trustpilot-filterpagina's, fora). Elke CSV-rij bevat de URL van de bron.

| Tool | Gebruikte bronnen (aantal rijen) | Niet gelukt / niet aanwezig | Kwaliteitsnoot |
|---|---|---|---|
| OutSmart | Google Play `com.werkbon` (40), App Store NL id1314341924 (35), Trustpilot out-smart.com (22, TrustScore 2,3), SoftwareWatcher (3) | Capterra 0 reviews; OutSmart Next-app 0 NL-reviews; prijspagina 404 | Goed. App-store-reviews alleen vanaf 2022 meegenomen (ca. 150 oudere weggelaten, zelfde beeld) |
| Simple-Simon | Google Play `com.mobileop` (28), App Store id897884395 (37) | Geen Trustpilot-profiel; G2 en Capterra niet opgehaald | Matig: veel oud en positief, mogelijk gestuurd |
| Gripp | Trustpilot (23, TrustScore 1,9), Capterra.com (15), App Store Time Tracker (3) | Google Play 404; G2 alleen als zoeksamenvatting | Redelijk; vooral bureaus |
| Workmate | Google Maps (19) | Trustpilot, app-stores, Capterra en G2: niets | Dun en positief geclusterd |
| Spotmaster | Google Play (1), Google Maps (1) | Trustpilot 404; Capterra, G2 en App Store: niets | Onbruikbaar |
| Tradecount | – | Site niet bereikbaar (502/time-out); geen product gevonden | Naam controleren (Tradify? Plancraft?) |
| WeFact | Trustpilot (73; profiel 266 reviews, 4,2), App Store (15), Google Play (9) | Capterra (1 review) niet opgehaald | Goed, met migratie-bias |
| BouwBit | – | Geen softwareproduct | Bedoeld: Bouw7 of Bouwflow? |
| Exact Bouw7 | Google Play `com.gobuildit.bouw7` (44), App Store id922818646 (21), Capterra.nl (4) | Capterra.com time-out; Trustpilot exact.com gaat over Exact algemeen (niet opgenomen) | Redelijk; recent dun |
| Syntess | App Store Syntess SARA (3) | Trustpilot 404; TrustRadius, Capterra en G2: niets; geen Google Play-app | Onbruikbaar; interviews nodig |
| KRAAN | App Store KRAAN Werkbon (1) | Trustpilot 404; Capterra: niets | Onbruikbaar |
| Admicom | – | Geen app, geen reviews (NL-entiteit is ECI Admicom; niet te verwarren met het Finse Admicom Oyj) | Geen data |
| Sollit | Google Play 2Solar (4), App Store (4), Capterra.nl (1), Trustpilot 2solar.es (4) | Trustpilot 2solar.nl en sollit.com: geen profiel; G2 en Capterra.com time-out | Zeer dun |
| Solar Monkey | – | Geen reviews op Trustpilot, Capterra, G2, Pipedrive Marketplace, Tweakers of Reddit; geen app | Alleen een profielschets |
| OpusFlow | Trustpilot (2), Capterra.ca (2) | G2-teksten niet leesbaar | Zeer dun |
| Teamleader Focus | Google Play (15), App Store NL (7) en BE (6), Trustpilot NL (39) en EN (2), Capterra.nl (5) | G2 mislukt; Capterra.com en OMR overgeslagen om credits te sparen | Goed voor app/prijs/lock-in; weinig vakbedrijven |
| Werkspot | Google Play "Werkspot voor Vakmensen" (32), App Store (23), Trustpilot NL (57) en EN (14), Radar-forum (3) | Kassa en Reddit: niets; Tweakers en LinkedIn niet doorzocht | Goed; negatieve filter-bias |
| Solvari | Trustpilot NL (34) | Geen vakman-app gevonden | Dun en verouderd |
| Trustoo | Trustpilot NL (54; profiel 4.738 reviews, 4,3, overwegend consumenten) | Vakman-app niet gevonden; prijspagina niet opgehaald | Recent, maar eenzijdig negatief |
| Zoofy | Google Play `nl.zoofy.mobile` (24), Trustpilot NL (14) | – | Redelijk; veel aanmeldklachten |
| Moneybird (P2) | App Store (25), Google Play (19), Trustpilot (17; score 2,2) | Capterra (1), G2 (14) en Feedback Company niet opgehaald | Redelijk; geen vakbedrijven herkenbaar |
| e-Boekhouden.nl (P2) | Google Play (18), App Store (9), Trustpilot (13; profiel 4,5 uit 2.069) | GetApp en Trustpilot-filters voor 1★/4★ niet opgehaald | Dun |
| SnelStart (P2) | App Store (19), Google Play (20), Trustpilot (10) | Prijspagina 404 (prijs uit secundaire bronnen) | Redelijk |
| Exact Online (P2) | App Store NL (37 uit 100 nieuwste), Google Play (30 uit 100), Trustpilot NL (7 uit 80) | Capterra.nl gaf 410/404 | Redelijk; alleen thema's facturatie/koppeling/app opgenomen |
| HubSpot (P2) | Capterra.com (4, bouw/facilities), HubSpot Community (1) | G2 time-out; Software Advice 404 | Indicatief; geen NL-reviewers |
| Pipedrive (P2) | Capterra.com (9, bouw/renewables) | G2 time-out; Reddit leverde niets op | Indicatief; geen NL-reviewers |

### Aanbevolen vervolgonderzoek
1. **Interviews** met 8–12 vakbedrijven (2–25 man) die Syntess, KRAAN, OutSmart of Simple-Simon gebruiken én leads van platforms kopen. Toets de gaten uit §4, die nu vooral uit afwezigheid zijn afgeleid.
2. **Tweakers, LinkedIn en Facebook-groepen** ("Ondernemende vakmensen", installateursgroepen) handmatig doorzoeken. Dat ging hier niet systematisch.
3. **Tradecount en BouwBit verifiëren** (juiste namen) en eventueel Tradify, Plancraft of Bouwflow toevoegen.
