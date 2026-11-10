# CONCEPTEN – kansen voor technische vakbedrijven (NL)

*Uitgewerkt op 10 november 2026. De basis is de review-analyse in deze repo: [`SAMENVATTING.md`](SAMENVATTING.md), `analyse/` en `data/` (26 tools, 981 reviews).*

**Hoe je dit leest.** Elk concept begint bij een pijn die in de reviews aantoonbaar terugkomt, met citaat en vindplaats. Alles wat níét uit de reviews komt is gemarkeerd als **[aanname]**: prijzen, betaalbereidheid, technische haalbaarheid en marktomvang. Die punten moeten nog gevalideerd worden; in §4 staan per concept goedkope tests. De werktitels zijn alleen labels.

---

## 0. Waar de kansen liggen: vier inzichten uit de reviews

1. **Het gevecht wordt gewonnen vóór de offerte, en daar heeft de vakman geen gereedschap.** Leads worden met 3–10 bedrijven gedeeld (lead-concurrentie 35×) en de klant is "binnen 1 uur" al weg (Trustoo, 2026-04-29). In 488 software-reviews komen lead-opvang, offerte-opvolging en WhatsApp samen nog geen 20 keer voor: de bestaande tools doen er niets mee.
2. **Vakmannen zijn niet tegen betalen, wel tegen betalen zonder resultaat.**
   - "Werkspot zou alleen een lead moeten berekenen wanneer iemand daadwerkelijk de opdracht krijgt." (Werkspot, Trustpilot, 2026-05-05)
   - "Als ik 150 zou moeten betalen per klant, geen enkel probleem" (Trustoo, 2026-01-31)
3. **De vakman bezit zijn eigen klantrelatie niet.** Die zit bij het platform ("na jaren ben ik dus al mijn contacten kwijt en recensies", Werkspot, installatiebedrijf, 2026-04-10) of zit opgesloten in software ("Dit voelt als een gijzeling", Gripp, 2025-01-09).
4. **Vertrouwen is het product.** De meest genoemde softwareklachten gaan niet over ontbrekende functies maar over betrouwbaarheid: bugs (132), de mobiele app (107), prijsverhogingen (61) en lock-in (36). Wie stabiel, voorspelbaar geprijsd en vrij-van-lock-in is, onderscheidt zich al.

Daaruit volgen drie terreinen met ruimte:

| Terrein | Wat er nu is | Gat |
|---|---|---|
| **Voordeur** (aanvraag → eerste contact → kwalificatie) | Leadplatforms die contact verkopen; mail en WhatsApp los op de telefoon | Snelheid, overzicht, rendement per bron, eigen kanaal |
| **Offerte → ja** | Boekhoud- en algemene CRM-pakketten; offertes zijn "net niet" voor maatwerk | Offerte op locatie + automatische opvolging |
| **Na de klus** (nazorg, onderhoud, reviews, herhaalwerk) | Alleen in zwaardere werkbon/ERP-tools (Simple-Simon, OpusFlow, Workmate) | Terugkerende omzet en eigen reputatie voor de 2–25-man-bedrijven |

Wat we **niet** moeten doen:
- **Werkbon, planning, ERP en boekhouding nabouwen.** Dat terrein is bezet, en de klachten gaan juist over hoe moeilijk het is om het goed te doen.
- **Meteen een algemeen leadplatform beginnen.** Dat wordt pas zinnig in de netwerkvorm van concept 7, en pas als er een gebruikersbasis is.

---

## 1. De concepten

### Concept 1 – "Eerste-reactie-assistent" (lead-inbox + directe reactie)

**Pijn (bewijs)**
- "als je een aanvraag krijgt per email en whatsapp en gelijk opent hebben 3 andere personen al gereageerd." (Trustoo, 2025-11-25)
- "27 leads … waarvan er 20 niet eens antwoorde op mijn eerste bericht, terwijl ik er altijd binnen 5 minuten bij was" (Trustoo, 2026-01-31)
- Teamleader-app: "niet geregistreerd dat je gebeld hebt", "geen push notificaties" (App Store, 2023)

**Concept**
- **Eén inbox voor alle aanvragen.** Leadmails van Werkspot, Trustoo en Solvari, websiteformulieren, WhatsApp Business, gemiste oproepen en Facebook/Google-berichten komen samen. Ze worden automatisch omgezet naar een lead met naam, adres, klus en bron.
- **Binnen 60 seconden een reactie namens de vakman.** Een persoonlijke WhatsApp of sms ("Dank je, ik ben Jan van Dakwerken X. Mag ik 3 foto's van het dak?"), met een belknop die het gesprek logt.
- **Een opvolgreeks als de klant niet reageert**, bijvoorbeeld na 2 uur, de volgende ochtend en na 3 dagen, via WhatsApp en sms afwisselend.

**Voor wie:** vakbedrijven die (ook) leads kopen, en eenmanszaken tot 10 man die alles zelf op hun telefoon doen.

**Waarom nu:** de leadprijzen stijgen ("rond de €20 … nu hedendaags €40", Werkspot, 2026-07-05) en Trustoo heeft sinds eind 2025 een extra Premium-bijdrage. Elke gemiste lead wordt duurder.

**Verdienmodel [aanname]:** €19–39 per maand per bedrijf, zonder minimum aantal gebruikers. De rekensom voor de klant: één extra gewonnen klus per kwartaal, of een paar leads die niet meer verloren gaan à €12,50–40 (de prijzen uit de reviews), betaalt het abonnement al.

**MVP**
- Een doorstuuradres voor leadmails (parser per platform) en een koppeling met WhatsApp Business.
- Een mobiele lijst met swipe-acties.
- Drie sjablonen per vak.

**Risico's**
- WhatsApp Business API: kosten per gesprek of bericht, eisen aan sjabloonberichten, en opt-in voor automatische berichten **[aanname: regels en tarieven van Meta verifiëren]**.
- Platforms kunnen het e-mailformaat veranderen, waardoor de parser het onderhoud waard moet blijven.
- Platformvoorwaarden kunnen contact buiten het platform beperken **[verifiëren per platform]**.

---

### Concept 2 – "Leadboekhouder" (rendement per bron + restitutie-dossier)

**Pijn (bewijs)**
- "Over maart hebben wij een openstaande rekening van € 1.244. Verwachte omzet van de leads is circa € 925." (Trustoo, 2026-03-28)
- "Reageert de consument niet? Klopt het 06 nummer niet? Helaas 99% van de tijd word je restitutie aanvraag geannuleerd" (Werkspot, 2026-10-30)
- Bij Solvari is de reclamatielimiet "meteen vol" (2025-12-26). Bij Trustoo word je volgens reviewers minder zichtbaar als je reclameert.

**Concept**
- **Per leadbron bijhouden wat het kost en wat het oplevert:** leadkosten (handmatig of uit de facturen van het platform), gereageerd, offerte, gewonnen, omzet. Het resultaat is een eenvoudig maanddashboard: "Werkspot: €410 uitgegeven, 2 klussen, €3.100 omzet. Trustoo: €380 uitgegeven, 0 klussen."
- **Restitutie-dossier.** Elke contactpoging wordt met tijdstempel gelogd: WhatsApp niet afgeleverd, gebeld zonder antwoord, nummer onjuist. Daaruit maakt het systeem met één klik een reclamatieverzoek.

**Waarom interessant**
- Het is een **instapproduct dat de vakman direct geld bespaart** en daarmee een natuurlijke voorkant voor concept 1.
- Het levert de data op die concept 7 nodig heeft: welke bron converteert echt.

**Verdienmodel [aanname]:** een gratis versie (handmatig leads en kosten invoeren) als lead-magnet, met de betaalde versie als onderdeel van concept 1. Eventueel een "no cure, no pay"-restitutieservice: een percentage van het teruggekregen bedrag.

**MVP:** het kan zelfs als spreadsheet-sjabloon plus WhatsApp-logging uit concept 1. Een concierge-test is mogelijk: zelf voor 5 vakmannen hun reclamaties schrijven.

**Risico's**
- Het is onbekend of platforms een gelogde contactpoging als bewijs accepteren **[aanname: testen]**.
- Platforms kunnen hun reclamatiebeleid aanpassen.

---

### Concept 3 – "Slimme intake + prijsindicatie" (de prijs-shopper eruit filteren)

**Pijn (bewijs)**
- "veel aanvragen uitsluitend bedoeld om een indicatie van de kosten te krijgen" (Werkspot, 2026-08-25)
- Klanten "laten je langskomen om een offerte op te maken om zo een ander bedrijf goedkoper te laten uitkomen" (Trustoo, 2025-11-18)
- Aanvragen te vaag om te prijzen (Werkspot); "betere omschrijving van de klus" (Zoofy); klanten vullen het aanvraagformulier onvolledig in (Pipedrive, Capterra.com)

**Concept**
- **Een intakelink of WhatsApp-flow per vak**, die de vakman op zijn website, Google-profiel en in reacties op leads zet. De klant beantwoordt 5–8 gerichte vragen (type dak, m², bouwjaar, foto's, gewenste periode, budgetbandbreedte).
- **Optioneel krijgt de klant direct een prijsindicatie** ("schilderwerk buitenkozijnen rijtjeshuis: €1.800–2.600"), gebaseerd op de eigen tarieven van de vakman.
- **De vakman ziet vooraf een score:** compleetheid, afstand, budget versus indicatie. Pas daarna besluit hij of hij langsgaat.

**Waarom het werkt:** wie alleen een prijs zoekt, krijgt die zonder dat de vakman rijdt. Wie overblijft, is serieuzer. De foto's en maten gaan meteen het dossier in voor de offerte (concept 4).

**Verdienmodel:** een onderdeel van concept 1 of 4. Eventueel apart als widget voor de website **[aanname]**.

**MVP:** 3 vakken (dakdekker, schilder, cv/warmtepomp) met elk een vragenlijst. De prijsindicatie is een eenvoudige tabel die de vakman zelf invult.

**Risico's**
- Een indicatie kan een verwachting scheppen waaraan de klant de vakman later houdt. Duidelijke disclaimers zijn nodig.
- Vakmannen willen hun prijzen misschien niet vooraf tonen **[aanname: valideren]**.

---

### Concept 4 – "Offerte aan de keukentafel" (maatwerk-offerte op locatie + opvolging)

**Pijn (bewijs)**
- "Je werkt letterlijk drie keer aan hetzelfde project om één offerte klaar te krijgen" (Teamleader, plaatser BE, 2026-08-10)
- "Als installateur maak ik hier ook mn offertes etc in maar dat werkt maar voor de helft." (Exact Online, installateur, 2026-11-02)
- "heb een iPad gekocht om klanten makkelijker te kunnen laten tekenen… dan is de app niet ingericht om op een iPad" (Moneybird)
- Offerte aanpassen in de app is een wens (Sollit, 2021); offertes versturen vanaf de iPhone ook (WeFact, 2020)
- Waardering voor het tegendeel: "precies zien hoe vaak mijn klanten de offerte hebben bekeken" (Teamleader, 2024-07-26); "Klanten kunnen met 1 klik hun samenwerking bevestigen" (Teamleader, 2025-03-05). Bij WeFact zitten deze functies alleen in het duurdere Plus-pakket.

**Concept**
- **Offerte op tablet of telefoon** met **calculatieblokken per vak**: m² dak, strekkende meter goot, aantal kozijnen, stelposten en meer- en minderwerk. Foto's uit de intake komen er direct in.
- **Ter plekke laten tekenen.**
- **Automatische opvolging:** een melding zodra de offerte is geopend, een herinneringsreeks via mail en WhatsApp, en na een "ja" een opdrachtbevestiging en aanbetalingslink.
- **Daarna doorzetten** naar het werkbonpakket en het boekhoudpakket: Moneybird, e-Boekhouden en Exact via hun API, SnelStart via UBL/Peppol. Volgens een reviewer kost de SnelStart-API de klant een upgrade naar €54 per maand plus €250 certificering.

**Waarom dit naast concept 1 de kern is:** de offerte is het moment waarop de lead omzet wordt. Opvolging is in de reviews het meest gewaardeerde CRM-onderdeel (Teamleader, Pipedrive: "ensures no follow-ups are missed"). Generieke pakketten missen de vakkennis.

**Verdienmodel [aanname]:** in het kernpakket. Expliciet **geen** "opvolging alleen in Plus", om ons af te zetten tegen WeFact.

**Risico's**
- Calculatie per vak is breed: begin met 2–3 vakken.
- Vakmannen met een vaste werkwijze in Excel hebben een import of sjabloon nodig.

---

### Concept 5 – "Nazorgmotor" (onderhoudsabonnementen en herhaalwerk)

**Pijn en vraag (bewijs)**
- Waar het bestaat, wordt het gewaardeerd: "Periodiek onderhoud aan machines is gemakkelijk in te plannen … geschiedenis gemakkelijk te bekijken" (Simple-Simon, App Store, 2023-11-20) en "checklists voor … ketelonderhoud" (OpusFlow, Trustpilot, 2026-07-07).
- Waar het ontbreekt, wordt het gemist: "kijken uit naar de jaarplanning die gaat komen" (Simple-Simon, 2022); geen "week/maandplanning … waarbij opdrachten en contracten wekelijks/maandelijks terugkeren" (Gripp, 2021); "niet kunt zien wat de vorige problemen waren met de machine" (OutSmart, 2022).
- Geen enkele tool koppelt nazorg aan omzet zoals herinneringen naar de klant, onderhoudscontracten of reviews. Dit volgt uit afwezigheid in de reviews, niet uit een expliciete vraag.

**Concept**
- **Per adres en per object** (cv-ketel, warmtepomp, zonnepanelen, dak, buitenschilderwerk) een onderhoudsinterval vastleggen.
- **Het systeem nodigt de klant automatisch uit** voor onderhoud of inspectie via WhatsApp of mail, met een planlink. Voorbeeld: "Uw dak is 2 jaar geleden geïnspecteerd; zullen we vóór de winter even kijken?"
- **Onderhoudsabonnementen** (bijvoorbeeld €X per jaar voor jaarlijks onderhoud plus voorrang bij storing) met automatische incasso.
- **Na elke klus een reviewverzoek** naar een eigen profiel, zie concept 6.

**Waarom interessant**
- Het geeft de vakman **terugkerende omzet** en maakt hem minder afhankelijk van betaalde leads (inzicht 2 en 3).
- Het is een **voor de hand liggende uitbreiding** op een klantdossier per adres.
- Waarschijnlijk de **grootste waarde per klant** **[aanname: dat bestaande klanten goedkoper te bedienen zijn dan nieuwe, is een algemeen marketingprincipe en hier niet gemeten]**.

**Verdienmodel [aanname]:** in een hoger pakket, of een klein percentage over abonnementsincasso's.

**MVP:** intervallen per object, plus een WhatsApp- of mailherinnering met een planlink. Zonder incasso.

**Risico's**
- Werkt alleen als het dossier gevuld is. Dat vraagt een import van oude klanten (adres + jaar + type werk).
- Per vak verschilt het hoe zinvol dit is: groot voor installateurs, middel voor dak en schilder, klein voor eenmalige verbouw **[aanname]**.

---

### Concept 6 – "Eigen voordeur" (eigen reviews, eigen kanaal, minder platformafhankelijk)

**Pijn (bewijs)**
- "Werkspot heeft mijn account geblokkeerd … na jaren ben ik dus al mijn contacten kwijt en recensies" (Werkspot, installatiebedrijf, 2026-04-10)
- Reviews op het profiel zijn waardevol, en daarom is een accountblokkade zo pijnlijk (analyse Werkspot)
- Bij Zoofy wordt de uitbetaling ingehouden bij een klacht (analyse Zoofy)

**Concept:** een pakket om eigen aanvragen binnen te halen zonder leadplatform.
- Een simpele vakpagina of mini-site met de intake uit concept 3.
- Synchronisatie met het Google-bedrijfsprofiel.
- Een WhatsApp-knop.
- Na elke klus een automatisch reviewverzoek (Google en een eigen reviewpagina).
- Een bron-tag "eigen kanaal" in het rendementsoverzicht uit concept 2. Zo ziet de vakman zwart op wit dat eigen aanvragen goedkoper zijn.

**Waarom interessant:** dit is het tegenmiddel tegen inzicht 3, en het is meetbaar met concept 2: "deze maand 40% van je klussen via je eigen kanaal, €0 leadkosten".

**Verdienmodel:** een onderdeel van het abonnement. Eventueel een aparte set-up-dienst **[aanname]**.

**Risico's**
- Er is veel concurrentie van websitebouwers en reviewtools. Het onderscheid zit alleen in de integratie met de inbox en het dossier.
- De regels van Google voor reviewverzoeken moeten gevolgd worden **[verifiëren]**.

---

### Concept 7 – "Eerlijk vakmannetwerk" (betalen per resultaat, en doorverwijzen tussen vakmannen)

**Pijn (bewijs)**
- "Werkspot zou alleen een lead moeten berekenen wanneer iemand daadwerkelijk de opdracht krijgt." (2026-05-05)
- "Als ik 150 zou moeten betalen per klant, geen enkel probleem" (Trustoo, 2026-01-31)
- Leads "buiten je gebied" (Trustoo, 2026-05-21) en filters die "niet werken zoals het hoort" (Trustoo, 2026-08-07)
- "exclusief" blijkt toch aan 7–10 bedrijven verkocht (Solvari)

**Concept, in twee stappen**
- **7a. Doorverwijsnetwerk tussen gebruikers.** Een lead die je niet kunt aannemen (buiten je vak, buiten je regio, of je agenda zit vol) stuur je met één tik door naar een collega in het netwerk. Je krijgt een vergoeding als die collega de klus wint. Dit is kleinschalig te starten, met de eigen gebruikers van concept 1.
- **7b. Leads op basis van resultaat.** Pas als er een gebruikersbasis is, ook consumentaanvragen verdelen. Dan **betaalt de vakman alleen bij een getekende offerte** (een vast bedrag of een percentage), en krijgt elke lead **maximaal 1–2 vakmannen**.

**Het onderscheidende punt:** leadplatforms rekenen per contact omdat ze niet kunnen zien of een klus doorgaat. Ons systeem kan dat wél, omdat de offerte in concept 4 wordt getekend. **Wie de offerte-ondertekening bezit, kan eerlijk per resultaat afrekenen.** Dit is de positie die bestaande leadplatforms niet zomaar kunnen innemen **[aanname: dat ze het niet kunnen of willen, is een inschatting]**.

**Risico's (groot)**
- Een marktplaats met twee kanten heeft een kip-en-ei-probleem.
- Fraude: de opdracht buiten het systeem afsluiten om de fee te ontlopen. Mogelijke tegenmaatregelen zijn een lage fee, voordelen voor wie binnen het systeem blijft (garantie, reviews) en steekproeven.
- Consumenten werven kost veel marketingbudget.
- Daarom pas na concept 1–4, en eerst als 7a.

---

### Concept 8 – "Overstap zonder pijn" (migratie, data-vrijheid en timing)

**Pijn (bewijs)**
- Prijsverhogingen: OutSmart ×3–4 in 2024; Gripp "de pan uit gerezen" na de overname door Exact (2025-06-27); de pakketwijziging van Moneybird in 2026.
- Lock-in: export voor €169 (Gripp), een jaarcontract met deurwaarder (Teamleader), "opzie tegen de mutatie van alle gegevens naar een vergelijkbaar systeem" (Teamleader, 2026-10-21).
- Onboarding is zwaar (42× in software). "we're paying quite a lot … but I honestly feel lost on how to use it" (HubSpot, dak-/bouwbedrijf, 2025-06-25). Een "teamleader expert aan 1250€ die amper iets heeft uitgevoerd" (Teamleader, 2024-07-17).

**Concept:** geen product maar **de manier van verkopen en het versterken van vertrouwen**.
- Gratis import uit Gripp, Teamleader, WeFact, OutSmart en Excel.
- "Ingericht in een dag" met vaksjablonen.
- Een **schriftelijke data-exitgarantie**: altijd gratis een volledige export, inclusief bijlagen.
- **Prijsgarantie**: bijvoorbeeld 24 maanden geen verhoging voor bestaande klanten **[aanname: commerciële keuze]**.
- Maandelijks opzegbaar.

**Timing als kans:** klanten zijn het meest bereid over te stappen vlak na een prijsverhoging. De Trustpilot-pieken rond OutSmart (nov 2024) en Gripp (na de Exact-overname) laten zien wanneer dat speelt. Een eenvoudige "overstapmonitor" op die signalen geeft acquisitiemomenten.

**Risico:** het is weinig onderscheidend als concurrenten hetzelfde gaan beloven. Daarom moet de garantie contractueel en geloofwaardig zijn.

---

### Kleinere kansen (dunne data, alleen noteren)

- **Koppellaag werkbon ↔ boekhouding.** "Koppeling … houtje touwtje werk" (Bouw7, 2023), de Exact-koppeling werkt "net niet" (OutSmart). Er bestaan al veel koppelingen en iPaaS-tools, dus het is beter als feature (concept 4) dan als apart product.
- **Snellere uitbetaling of voorfinanciering voor platformvakmannen.** Bij Zoofy komt de uitbetaling volgens reviewers maanden te laat (7×). Het is een niche en de data is dun.
- **Interne WhatsApp-nudges voor het team** ("Nog beter als er een WhatsApp komt als je week uren niet kompleet zijn", Bouw7, 2023). Klein, maar het past in dezelfde WhatsApp-laag.

---

## 2. Vergelijking

De scores zijn mijn inschatting op basis van de reviews, op een schaal van 1–5. Bij concurrentie betekent 5 veel open ruimte; bij haalbaarheid betekent 5 snel te bouwen.

| # | Concept | Bewijs van pijn | Ernst (geld of klant) | Open ruimte | Haalbaarheid | Versterkt de rest | Totaal |
|---|---|:-:|:-:|:-:|:-:|:-:|:-:|
| 1 | Eerste-reactie-assistent | 5 | 5 | 4 | 4 | 5 | **23** |
| 2 | Leadboekhouder | 4 | 5 | 5 | 5 | 4 | **23** |
| 3 | Slimme intake + prijsindicatie | 4 | 4 | 4 | 4 | 4 | **20** |
| 4 | Offerte aan de keukentafel | 4 | 4 | 3 | 3 | 5 | **19** |
| 5 | Nazorgmotor | 3 | 3 | 4 | 3 | 4 | **17** |
| 6 | Eigen voordeur | 3 | 4 | 2 | 4 | 4 | **17** |
| 8 | Overstap zonder pijn | 4 | 3 | 3 | 4 | 3 | **17** |
| 7 | Eerlijk vakmannetwerk | 4 | 5 | 4 | 1 | 3 | **17** |

**Toelichting**
- **Concept 1 en 2** hebben het sterkste bewijs (225 vakman-reviews over leadplatforms) en zijn relatief klein te bouwen.
- **Concept 4** is de noodzakelijke kern, maar scoort lager op open ruimte omdat offertetools bestaan; het onderscheid zit in vakkennis en opvolging.
- **Concept 7** heeft de grootste potentie maar is het moeilijkst, en hangt af van 1 en 4.
- **Concept 5** heeft vooral bewijs via afwezigheid en moet het eerst in interviews bewijzen.

---

## 3. Aanbevolen route: één product, in lagen

**Werktitel:** "de voordeur en het geheugen van het vakbedrijf". Het product zit vóór de werkbon (de aanvraag) en ná de werkbon (de nazorg), en koppelt met wat de vakman al heeft.

| Fase | Wat | Concepten | Belofte aan de vakman | Waarom deze volgorde |
|---|---|---|---|---|
| **1. Instap** | Lead-inbox, directe WhatsApp-reactie, rendement per bron, intake | 1 + 2 + 3 | "Geen betaalde lead meer verloren door traagheid, en je ziet wat elk platform je echt oplevert." | Sterkste en meest recente pijn, snel waarde, direct meetbaar in euro's |
| **2. Kern** | Offerte op locatie, opvolgreeks, digitaal tekenen, klantdossier per adres, koppeling met boekhouding | 4 (+8 voor de verkoop) | "Van aanvraag tot getekende offerte in één app die gewoon werkt." | Zet leads om in omzet; het ondertekeningsmoment maakt fase 4 mogelijk |
| **3. Groei** | Nazorgmotor, onderhoudsabonnementen, eigen reviews en voordeur | 5 + 6 | "Je bestaande klanten brengen je volgende klus." | Minder afhankelijk van platforms; terugkerende omzet |
| **4. Netwerk** | Doorverwijzen, later leads op basis van resultaat | 7 | "Betaal alleen voor klussen die je wint." | Kan pas met gebruikers en conversiedata uit fase 1–2 |

**Positionering over alle fases heen**, rechtstreeks volgend uit de grootste softwareklachten:
1. **Betrouwbaarheid als belofte.** Geen updates die data wissen, een app die ingelogd blijft, een offline wachtrij. (bugs 132×, mobiel 107×)
2. **Eerlijke prijs.** Per bedrijf, geen minimum van 2 gebruikers, opvolging niet als duurdere add-on, maandelijks opzegbaar, prijsgarantie. (prijs 61×)
3. **Jouw data, jouw klanten.** Gratis volledige export en een eigen reviewprofiel. (lock-in 36×; account geblokkeerd = recensies kwijt)
4. **Persoonlijke, bereikbare support.** (de nummer-2-waardering, 58×)

---

## 4. Validatieplan (± 6–8 weken, laag budget)

| Week | Test | Concept | Succescriterium (voorstel) |
|---|---|---|---|
| 1–2 | **12 interviews** met vakbedrijven van 2–25 man (mix dak, schilder, installatie), van wie de helft leads koopt. Vraag naar de laatste 10 aanvragen: bron, reactietijd, uitkomst en kosten. | allemaal | ≥ 8 van 12 noemen trage opvolging of leadkosten zonder dat je ernaar vraagt |
| 1–2 | **Concierge-leadboekhouder:** voor 5 vakmannen hun leadkosten en uitkomsten van de afgelopen 3 maanden in een sheet zetten, plus voor hen restituties indienen | 2 | Minstens één vakman krijgt aantoonbaar geld terug; ≥ 3 van 5 willen het blijven gebruiken |
| 2–4 | **WhatsApp-reactiepilot:** 3–5 vakmannen sturen hun leadmails door; wij reageren (eerst handmatig of half-automatisch) binnen 2 minuten met intakevragen | 1 + 3 | Reactietijd < 5 minuten; hoger aandeel "klant reageert terug" dan hun eigen nulmeting |
| 3–5 | **Landingspagina's** per belofte (A: "nooit meer een lead kwijt", B: "betaal alleen voor gewonnen klussen", C: "je oude klanten brengen je nieuwe klus") met een wachtlijst; gerichte advertenties per vak | 1, 7, 5 | Conversie naar wachtlijst per variant; welke belofte trekt |
| 4–6 | **Prototype offerte op tablet** voor 1 vak (dakdekker of schilder), testen aan een echte keukentafel | 4 | Offerte in < 15 minuten ter plekke; de vakman wil het bij een volgende klant weer gebruiken |
| 6–8 | **Betaalbereidheid:** pre-sale of een "founding member"-prijs | 1 + 2 + 4 | ≥ 10 bedrijven betalen vooruit of tekenen een intentie |

**Nog uit te zoeken (feiten, niet aannemen)**
- WhatsApp Business Platform: tarieven per bericht of gesprek in NL, regels voor sjablonen en opt-in, en de wachttijd voor goedkeuring.
- Voorwaarden van Werkspot, Trustoo en Solvari: mag je leadmails automatisch verwerken en de klant buiten het platform benaderen?
- De mate waarin platforms een gelogde contactpoging als bewijs bij restitutie accepteren.
- Het aantal technische vakbedrijven van 2–25 man in NL per branche (CBS / KvK-SBI-codes), om de marktomvang te bepalen. Dit is niet in dit onderzoek bepaald.
- De API's en kosten van Moneybird, e-Boekhouden, Exact Online en SnelStart, en UBL/Peppol als alternatief.
