# WERKSPOT-ALTERNATIEF – concept voor een betere variant (deel 4)

*Opgesteld 10 november 2026. Gebaseerd op [`analyse/werkspot-diepte.md`](analyse/werkspot-diepte.md) (deel 1–3: feiten, 432 reviews van vakman en consument, benchmark van 14 platforms), [`SAMENVATTING.md`](SAMENVATTING.md) en [`CONCEPTEN.md`](CONCEPTEN.md).*

*Aanduidingen in dit document:*
- **[aanname]**: komt niet uit een bron en moet getest worden.
- **[interpretatie]**: mijn duiding van een bron.
- Tellingen verwijzen naar `data/werkspot.csv`: 191 vakman-rijen en 230 consument-rijen.

---

## Samenvatting

**Vakmannen en consumenten klagen over hetzelfde mechanisme, alleen vanaf twee kanten.** De vakman betaalt zodra de klant zijn contactgegevens deelt, ook als er geen opdracht uit komt (AV art. 19.1). Dat werkt als volgt:
1. Vakmannen worden selectief en reageren minder.
2. Consumenten krijgen te weinig reacties (te-weinig-reacties: 14 van 66 middenreviews) en nodigen meer bedrijven uit.
3. Leads worden met meer vakmannen gedeeld (lead-concurrentie 39×), waardoor de conversie daalt.
4. De leadprijs voelt daardoor nog hoger (leadkosten 159×, leadprijs 92×).

Aan de consumentenkant is de grootste pijn niet het platform maar **vertrouwen**: slechte vakmannen (48×), fraude met aanbetalingen (32×), geen screening (29×) en geen hulp bij een conflict (20×).

**Een betere variant doorbreekt beide tegelijk:**
1. Hooguit 3 vakmannen per aanvraag, gekozen door de consument.
2. Een gestructureerde intake met een verifieerbaar telefoonnummer.
3. De vakman betaalt pas na een stap die het platform zelf kan waarnemen. Eerst is dat een bevestigde afspraak, later een getekende offerte in onze offertetool.
4. Automatische terugbetaling op objectieve regels.
5. Gescreende vakmannen, optionele geldbescherming en reviews die alleen bij echte klussen horen en waarvan de vakman eigenaar blijft.

**De volgorde is cruciaal.** Begin niet als marktplaats maar als **tool voor de vakman** (concept 1, 2 en 4). Die tool levert eigen klanten, eigen reviews en de waarneembare "getekende offerte" op die betalen per resultaat mogelijk maakt. De marktplaats komt pas daarna, per regio en per vak.

---

## 1. De 10 grootste frustraties (vakman + consument)

**Hoe de score werkt:**
- **Frequentie** = het aantal reviews met dit thema, aan één kant of aan beide samen (bron: tellingen in deel 2).
- **Ernst** 3 = kost direct geld of veiligheid; 2 = kost tijd of vertrouwen; 1 = ergernis.
- **Score** = frequentie × ernst. Dit is een rangorde, geen meting van hoe vaak iets in de hele markt voorkomt, want de reviews zijn negatief vertekend (zie deel 2.7).

| # | Frustratie | Kant | Freq. | Ernst | Score | Bewijs (citaat, bron, datum) |
|---|---|---|---:|:-:|---:|---|
| 1 | **Betalen voor contact, niet voor werk** | vakman | 159 | 3 | 477 | "pas de lead te laten betalen door ondernemer nadat de klus gegarandeerd doorgaat" (Trustpilot NL, 2026-05-17); AV 19.1: "Het is niet nodig dat de Vakman de opdracht krijgt toegewezen" |
| 2 | **Leadkwaliteit**: klant reageert niet, fout nummer, prijs-shoppers | vakman | 81 (waarvan 47 reageert niet, 16 prijs-shoppers, 9 fout nummer) | 3 | 243 | "2 op 5 … alleen een berichtje van we hebben al iemand gevonden … wel een leadprijs" (Trustpilot NL, 2025-05-25, 2★) |
| 3 | **Leadprijs uit verhouding** tot de klus, en zonder aankondiging te wijzigen | vakman | 92 | 2 | 184 | "Voor een koffietafel enkel een nieuwe laklaag is er een commisie van 37 euro" (App Store, 2024-11-01, 2★); AV 19.7: wijzigbaar "te allen tijde en zonder nadere aankondiging" |
| 4 | **Slechte vakman of no-show** | consument | 48 + 21 | 2 | 138 | "Nagenoeg alle reacties bleken helemaal niet de bevoegdheid te hebben om het werk uit te voeren." (Trustpilot NL, 2026-07-13, 3★) |
| 5 | **Fraude en geen hulp bij een conflict** | consument | 32 + 20 | 3 | 156 | "Werkspot doet niets en verwijst mij door naar het Juridisch loket. … Ben overgestapt naar Klusup … omdat alle betalingen via Klusup gaan." (Trustpilot NL, 2025-12-03) |
| 6 | **Support onbereikbaar, restitutie afgewezen** | vakman | 67 (+28 restitutie) | 2 | 134 | Restitutie alleen als platformtegoed (AV 19.2); "99% van de tijd word je restitutie aanvraag geannuleerd" (Trustpilot NL, 2026-10-30) |
| 7 | **Spiraal van concurrentie en te weinig reacties** | beide | 39 + 16 | 2 | 110 | Vakman: "meer dan 200 klanten aangeschreven. Resultaat? Slechts 4 opdrachten en … bijna €1000 kwijt" (2025-08-07). Consument: "Van de 10 bedrijven … maar 3 gereageerd … bedrijven die reageren sowieso … een bedrag moeten betalen" (2026-10-02, 3★) |
| 8 | **Geen screening, nep- of onbetrouwbare reviews** | consument | 29 + 8 + 13 | 2 | 100 | "Een bedrijf dat zich voor het eerst aanmeldt … mag zelf voor de eerste 5 reviews zorgen … Dit betekent dus dat deze heel goed nep kunnen zijn!" (2025-03-15) |
| 9 | **Prijsonzekerheid** voor de consument | consument | 21 | 2 | 42 | Rekening hoger dan afgesproken, geen prijsindicatie (deel 2.4) |
| 10 | **Het model is onzichtbaar of voelbaar**: consument weet niet dat contact geld kost, wordt bestookt met mails | beide | 16 + 8 + 16 | 1 | 40 | "werkspot moet als koptekst aan consumenten laten weten dat 'chat starten' vakmensen geld kost!!" (2026-07-05); "spammen met de vraag om een review terwijl de klus pas maanden later zou plaatsvinden" (2026-10-16, 4★) |

Net buiten de top 10, maar hoog in ernst: **account geblokkeerd = reviews en contacten kwijt** (8×, ernst 3). "na jaren ben ik dus al mijn contacten kwijt en recensies" (Trustpilot NL, 2026-04-10). AV 11.2: na beëindiging "geen technische en/of contractuele toegang meer".

**Wat beide kanten waarderen** (de lat die we minstens moeten halen):
- **Snel een match en volume:** consument `positief:snelheid` 37, `positief:keuze` 11; vakman "Ik krijg redelijk veel klanten" (2025-05-25).
- **Het concept**, zonder eigen marketing: "Op zich een mooi platform voor mensen die niet zo goed zijn in netwerken" (vakman, 2025-03-04).
- **Reviews als vertrouwensanker:** "Na een selectie kan ik met gerust hart obv reviews, de klus uit handen geven." (consument, 2026-10-07, 5★)
- **Gemak en een werkende chat/app:** `positief:gemak` 20.

Over de prijs is geen van beide kanten positief.

---

## 2. Ontwerpprincipes

Elk principe gaat terug op een frustratie (F1–F10, zie §1) of een waardering (W). Waar mogelijk staat erbij welk ander platform het al zo doet.

| # | Principe | Lost op | Bewijs en voorbeeld elders |
|---|---|---|---|
| P1 | **Betalen pas na een stap die het platform waarneemt**: eerst een door beide bevestigde afspraak (schouw of opname), later een getekende offerte | F1, F2, F7 | Vakmanwens "beide mee eens … om gegevens te delen" (2025-01-15). De Thumbtack-pilot "betalen bij boeking" gaf "higher profits because the leads were highly qualified" (2025), maar stopte (deel 3.3) |
| P2 | **Maximaal 3 vakmannen per aanvraag, de consument kiest**, en de vakman ziet hoeveel anderen er al reageerden | F7 | "MAXIMAAL 3 TOT 4 MAN" (vakman, 2026-02-18); "Vroeger kon je ook nog filteren op aantal reacties" (2025-08-29); Angi gaat naar "homeowners choose", max 5 (CEO-brief, dec. 2024) |
| P3 | **Een gestructureerde intake per vak** (foto's, maten, periode, budgetband) en een **geverifieerd telefoonnummer**, plus voor de consument **direct een prijsindicatie** | F2, F9 | Vakmanwens "strengere eisen … aan de volledigheid van aanvragen" (2026-09-05); MyBuilder verifieert elk telefoonnummer (FAQ 2023). Een prijsindicatie trekt de prijsvergelijkers weg [aanname] (zie CONCEPTEN concept 3) |
| P4 | **Automatische terugbetaling op objectieve regels, in geld en niet alleen als tegoed**: geen reactie van de consument binnen 72 uur, nummer onbereikbaar (gelogde belpogingen), afspraak niet nagekomen | F6 | Thumbtack: automatische refund bij geen reactie binnen 72 uur (deel 3); Werkspot: alleen tegoed, "Werkspot bepaalt geheel" (AV 19.2) |
| P5 | **Vakmannen screenen** (KvK, ID, aansprakelijkheidsverzekering, vakcertificaten waar relevant) en dat zichtbaar maken als badge | F4, F8 | Consumentenwens "Goed screenen is noodzaak" (2025-04-04, 3★); Checkatrade controleert vooraf; Homedeal-case met valse certificaten (deel 3) |
| P6 | **Optionele geldbescherming**: een aanbetaling of eindbetaling via het platform met bewaring tot oplevering, plus **bemiddeling bij een geschil** | F5 | "alle betalingen via Klusup" als reden om over te stappen (2025-12-03); Airtasker-escrow; Checkatrade-garantie tot £1.000 (deel 3). Of escrow juridisch mag (vergunning, betaaldienst via een PSP) is een [aanname] die we moeten toetsen |
| P7 | **Reviews alleen bij geverifieerde klussen, met hoor en wederhoor, en de vakman blijft eigenaar** (export, op zijn eigen site te tonen) | F8, en account geblokkeerd | "reviews splitsen in klant/vakman", hoor en wederhoor (vakman, 2025-08-13); MyBuilder accepteert alleen feedback van via het platform geworven klanten; tegenover Werkspot AV 11.2 (toegang weg na beëindiging) |
| P8 | **Open over het model naar de consument, en geen spam**: "Elke vakman betaalt pas als jullie een afspraak bevestigen"; een reviewverzoek pas na de klus; uitschrijven kan | F10 | Vakman (2026-07-05) en consument: "zonder dat je je schuldig hoeft te voelen" (2024-12-30) |
| P9 | **Voorspelbare kosten**: een maandplafond, per direct opzegbaar, prijswijziging minstens 30 dagen vooraf, de prijs zichtbaar vóór je reageert | F3, F6 | FixMyCar stapte over op een vast bedrag voor "greater certainty" (2026); Homedeal Pay Per Pick zonder minimale looptijd; Werkspot-AV 19.7 als tegenvoorbeeld |
| P10 | **Herhaalwerk en eigen klanten zijn gratis**: een fee alleen op de *eerste* klus met een via ons geworven klant | Omzeiling, en W reviews | Treatwell-achtig model (niet geverifieerd, deel 3.3). Dit maakt omzeilen minder aantrekkelijk en sluit aan op de nazorg in CONCEPTEN concept 5 [aanname] |
| P11 | **Bereikbare, menselijke support**, telefonisch | F6 | Vakmanwens "bereikbare support (telefoon)" (2025-08-27); support is in alle eerdere analyses een top-waardering |
| P12 | **Snelheid en volume behouden** (W): een push binnen een minuut naar de 3 gekozen vakmannen, een termijn voor reageren, daarna doorschuiven | W snelheid, F7 | Consumenten waarderen snelheid (37×); MyBuilder schuift na 24 uur door naar een grotere groep (deel 3) |

---

## 3. Alternatieve verdienmodellen

**Ankerpunten uit de bronnen**
- Vakmannen betalen nu €3–75 per lead bij Werkspot (FAQ, deel 1) en €12,50–40 per aanvraag bij Trustoo.
- Ze zeggen bereid te zijn meer te betalen per échte klant: "Als ik 150 zou moeten betalen per klant, geen enkel probleem" (Trustoo, 2026-01-31).
- Alle bedragen hieronder zijn **[aanname]** en moeten getest worden.

### Model A – "Betalen per bevestigde afspraak"
- **Hoe het werkt:**
  - De consument kiest maximaal 3 vakmannen.
  - De vakman ziet de intake gratis en reageert met een voorstel voor een tijdslot.
  - De vakman betaalt pas als beide kanten een afspraak bevestigen (opname of schouw).
  - Als de consument niet komt opdagen of de afspraak binnen 24 uur annuleert, krijgt de vakman het geld automatisch terug.
  - Voor kleine klussen zonder bezoek telt een bevestigde "akkoord op indicatie" als de afspraak.
- **Prijs [aanname]:** een vast bedrag per afspraak naar klusbandbreedte, bijvoorbeeld €15 / €35 / €60. De prijs staat vooraf bij de lead.
- **Voordelen:**
  - Het platform kan de stap zelf waarnemen: agenda, bevestiging door beide en eventueel een check-in.
  - Dicht bij wat vakmannen vragen ("beide mee eens").
  - Voorspelbaar en eenvoudig uit te leggen.
- **Nadelen:**
  - Een afspraak is nog geen opdracht, dus prijsvergelijkers blijven deels mogelijk. P3 (intake + indicatie) moet dat dempen.
  - Thumbtack stopte een vergelijkbare pilot vanwege "pain points" en ROI (deel 3.3).
- **Omzeiling beperken:**
  - Contactgegevens pas na een bevestigde afspraak.
  - Gemaskeerd nummer en chat in het platform tot dan (Thumbtack-aanpak).
  - Garantie, geldbescherming en een review alleen bij een afspraak via het platform.
  - Een lage prijs per afspraak maakt omzeilen weinig lonend.

### Model B – "Succesfee op getekende offerte"
- **Hoe het werkt:**
  - De vakman betaalt niets voor contact of afspraak.
  - Hij betaalt een fee zodra de consument de offerte digitaal tekent in onze offertetool (CONCEPTEN concept 4).
  - De fee geldt alleen voor de **eerste** opdracht van een via ons geworven klant; herhaalwerk is gratis (P10).
- **Prijs [aanname]:** gestaffeld naar offertewaarde, met plafond. Bijvoorbeeld 3–5% met minimaal €25 en maximaal €150–250. Dat sluit aan op "150 per klant, geen probleem".
- **Voordelen:**
  - Het model waar vakmannen het meest om vragen.
  - De prikkels van platform en vakman lopen gelijk.
  - De consument hoeft zich niet schuldig te voelen (F10).
- **Nadelen:**
  - **Het resultaat is alleen te zien als de offerte via ons getekend wordt.** Bij grote renovaties gaat onderhandelen vaak offline [aanname].
  - Vakmannen haten onvoorspelbare variabele kosten (FixMyCar 2026: "variable job fees do not work"; hipages NZ stapte af van de succesfee, deel 3.3).
  - De cashflow komt later voor ons.
- **Omzeiling beperken:**
  1. Contactgegevens pas na een bevestigde afspraak.
  2. Geldbescherming en garantie alleen bij tekenen en betalen via ons (zoals Klusup volgens zoekresultaten doet; **niet geverifieerd**).
  3. Een korte enquête bij de consument na 2 en 6 weken ("Heeft u een vakman gekozen? Wie?"); bij een afwijking een fee met waarschuwing.
  4. Reviews en zichtbaarheid alleen opbouwen via klussen op het platform.
  5. Een redelijk plafond, zodat eerlijk melden goedkoper is dan het risico op uitsluiting.
  6. De offertetool is ook buiten de marktplaats nuttig, dus de vakman gebruikt die tool tóch.
- **Wanneer:** pas als vakmannen de offertetool voor hun eigen klanten gebruiken (fase 2 in §5).

### Model C – "Hybride lidmaatschap met plafond" (aanbevolen startmodel)
- **Hoe het werkt:**
  - Een laag maandbedrag, inclusief de vakman-tools: inbox, eerste reactie, leadboekhouder en offerte.
  - Daarbij een **bundel bevestigde afspraken per maand** (model A) met maximaal 3 vakmannen per aanvraag en automatische terugbetaling.
  - Extra afspraken tegen een vast tarief, met een **maandplafond dat de vakman zelf instelt**.
  - Per direct opzegbaar.
  - Optioneel kan de vakman voor grote klussen kiezen voor model B in plaats van A.
- **Prijs [aanname]:** bijvoorbeeld €29–49 per maand inclusief tools en 2–3 afspraken, daarboven €15–60 per afspraak.
- **Voordelen:**
  - Voorspelbaar (P9, de FixMyCar-les).
  - De tool-inkomsten dragen de onderneming ook als de marktplaats nog dun is.
  - Het lidmaatschap filtert serieuze vakmannen (zoals Checkatrade).
  - Het geeft een sterk argument voor overstappen: "je betaalt nu €40 per contact, bij ons per afspraak".
- **Nadelen:**
  - Je betaalt nog steeds zonder garantie op een opdracht, al is het risico kleiner en begrensd.
  - Een abonnement kan aanvoelen als de klachten over Solvari en Trustoo.
  - Daarom geen jaarcontract en geen stilzwijgende verlenging.
- **Omzeiling beperken:** als bij A. Het lidmaatschap maakt omzeilen minder lonend, omdat de afspraken toch al in de bundel zitten.

**Vergelijking**

| | A: per afspraak | B: succesfee | C: hybride (start) |
|---|:-:|:-:|:-:|
| Lost F1 op (betalen zonder werk) | deels | **ja** | deels |
| Waarneembaar voor het platform | **ja** | alleen via onze offertetool | **ja** |
| Voorspelbaar voor de vakman | ja | nee | **ja** |
| Risico op omzeiling | laag–middel | **hoog** | laag |
| Inkomsten als de marktplaats nog dun is | laag | zeer laag | **middel (tools)** |
| Bewijs elders | Thumbtack-pilot (gestopt) | hipages en FixMyCar (teruggedraaid); werkt waar het platform de betaling doet (Zoofy, Airtasker) | Checkatrade (lidmaatschap), Homedeal (Pay Per Pick) |

**Advies:**
1. Start met **C**.
2. Test **B** als pilot bij 10–20 vakmannen zodra de offertetool gebruikt wordt.
3. Meet zowel omzeiling (enquête versus gemeld) als tevredenheid.

---

## 4. Het kip-en-ei-probleem

**Uitgangspunt: begin met de vakmannen, als tool die zonder marktplaats al waarde heeft.**

Het bewijs:
- Vakmannen klagen over kosten en tooling. Een tool lost dat zonder consumenten al deels op (concept 1 en 2: geen gemiste leads, rendement per bron).
- Jobber en Housecall Pro groeiden als software die leads van álle bronnen in één inbox trekt (deel 3).
- De CEO van hipages: "60% of work is generated by word of mouth" (Stockhead, 2024).

Een vakman met onze tool brengt zijn eigen klanten, eigen reviews en eigen intakelink mee. **Die klanten vormen de eerste vraagkant.**

**Stappen**
1. **Eén regio en 2–3 vakken die elkaar aanvullen [aanname, kiezen op basis van interviews].** Criteria:
   - frequente vraag;
   - klussen van €500–5.000, groot genoeg voor een fee en klein genoeg voor een snelle beslissing;
   - een intake op foto's werkt goed;
   - het ene vak verwijst vaak door naar het andere.
   Kandidaten: dakdekker + loodgieter/cv-installateur + schilder. Dakdekkers hebben urgente lekkages, installateurs terugkerend onderhoud (koppeling met de nazorg in concept 5), schilders seizoenswerk. Regio: daar waar de eerste 20–30 vakmannen uit de interviews en pilots zitten, liefst één stad met randgemeenten zodat er binnen 30 km genoeg aanbod is.
2. **Doorverwijzen tussen eigen gebruikers (concept 7a).** Vakmannen sturen klussen door die ze niet kunnen aannemen: buiten hun vak, buiten de regio of een volle agenda. Ze krijgen een vergoeding als de collega de klus wint. Zo komt er vraag op het platform zonder één euro voor consumentenwerving. Het bewijs dat zulke "verkeerde" leads bestaan: "buiten je gebied" (Trustoo, 2026-05-21); bij Werkspot noemen 16 vakmanreviews prijsvergelijkers en 1 een lead buiten het werkgebied (ondergrens, deel 2.2).
3. **De vraagkant werven zonder groot advertentiebudget [aanname, per kanaal testen]:**
   - **Pagina's met geverifieerde reviews per vakman en plaats** ("dakdekker in X", alleen echte klussen), voor organisch zoekverkeer. Werkspot heeft hier een grote voorsprong: 843.038 reviews en 6,8 miljoen klussen volgens de site (deel 1). Onze kans zit in de long-tail per regio, niet in de breedte.
   - **Elke offerte en factuur van een gebruiker** krijgt "Ook een andere vakman nodig? Wij kennen betrouwbare collega's". Dat gaat naar het netwerk.
   - **Partners met een terugkerende klusvraag:** VvE-beheerders, kleine verhuurders, makelaars (nieuwe eigenaren), verduurzamingsloketten en energiecoaches van gemeenten, lokale bouwmarkten. Ook Gamma en Praxis hebben een klusservice; dat zijn concurrenten of partners [aanname].
   - **Lokale gemeenschappen:** buurt-apps, Facebook-groepen per wijk en wijkkranten, met een simpele intakelink.
   - **De vertrouwensbelofte als boodschap:** "Max. 3 gescreende vakmannen, je geld beschermd tot oplevering". Dat speelt in op wat consumenten het hardst missen (F4, F5, F8).
4. **Pas daarna betaalde acquisitie**, en alleen per regio, als de verhouding tussen vraag en aanbod klopt. Meet de reactiegraad naar de consument (≥ 2 van 3 gekozen vakmannen reageren binnen 24 uur) en het aandeel afspraken.

**Liquiditeitsregel [aanname]:** open een vak in een regio pas voor consumenten als er minstens 8–10 actieve, gescreende vakmannen zijn. Zo kan elke aanvraag 3 goede reacties krijgen, en voorkom je de klacht "te weinig reacties" die Werkspot nu heeft.

---

## 5. Aansluiting op `CONCEPTEN.md`

| Fase | Concepten | Rol in het alternatief voor Werkspot |
|---|---|---|
| **1. Tool voor de vakman** | **1** (eerste-reactie-assistent), **2** (leadboekhouder), 3 (intake), 6 (eigen voordeur) | Vakmannen binnenhalen zonder marktplaats. Concept 2 bewijst zwart op wit wat Werkspot en Trustoo kosten per gewonnen klus, en dat is het overstapargument. De intake (3) wordt later de standaard-aanvraag op de marktplaats |
| **2. Offerte en dossier** | **4** (offerte aan de keukentafel) | Maakt de getekende offerte waarneembaar en is daarmee voorwaarde voor model B. Bouwt het klantdossier dat bij de vakman blijft (P7, P10) |
| **3. Netwerk** | **7a** (doorverwijzen) | De eerste vraagkant zonder advertentiebudget |
| **4. Marktplaats** | **7b** = dit document | Consumentenaanvragen met max 3 vakmannen, model C, en later B |
| Doorlopend | 5 (nazorgmotor), 8 (overstap zonder pijn) | Herhaalwerk is gratis (P10) en houdt vakmannen op het platform; overstappen van Werkspot wordt makkelijk gemaakt |

**Juridische randvoorwaarde voor concept 1 en 2** (uit deel 1):
- Werkspot-AV art. 6.14 (maart 2026) verbiedt "bots, scrapers of andere geautomatiseerde middelen om toegang te krijgen tot het Platform of gegevens daarvan te verzamelen, noch databases opbouwen uit Platformgegevens".
- Art. 6.10 + 6.15 leggen €1.000 boete per gebeurtenis op bij het omzeilen van de leadprijs.
- **Gevolgen voor het ontwerp:**
  - **Geen** automatische koppeling die inlogt op het Werkspot-account.
  - Alleen werken met wat de vakman zelf ontvangt en zelf invoert of doorstuurt (zijn eigen e-mail, zijn eigen kosten).
  - De tool mag nooit helpen de leadprijs te ontwijken.
- Of het verwerken van leadmails in de eigen mailbox onder "databases opbouwen uit Platformgegevens" valt, is **onzeker [interpretatie]**. Dit moet juridisch getoetst worden vóór de bouw. Dezelfde toets is nodig voor de voorwaarden van Trustoo en Solvari (niet onderzocht).

---

## 6. Wat Werkspot waarschijnlijk doet, en waar ze moeilijk kunnen volgen

**Wat ze al doen of waarschijnlijk zullen doen [interpretatie, op basis van deel 1 en 3]:**
1. **De consument laten kiezen, met een maximum aantal vakmannen.** Moederbedrijf Angi voerde dat in de VS in (max 5) en noemt een "comparable change in our European business" (CEO-brief, dec. 2024). Ons verschil in het aantal vakmannen per lead is dus kopieerbaar. Een maximum van 3 is scherper, maar niet uniek.
2. **De voorwaarden aanscherpen.** Dat gebeurde al in maart 2026: anti-scraping (6.14), anti-omzeiling met boete (6.10/6.15), één account en geen herregistratie (9.6A/B).
3. **Lokaal acties en kortingen** in onze startregio, bijvoorbeeld gratis tegoed (Werkspot deed eerder een cashback-actie, deel 1).
4. **Verificatie of een garantie toevoegen** voor consumenten. Dat is kopieerbaar, maar kost geld.
5. **Hun voorsprong in bereik en zoekmachines inzetten:** 42.491 vakmensen, 843.038 reviews en 6,8 miljoen klussen volgens de eigen tellers (deel 1).

**Waar ze moeilijk kunnen volgen [interpretatie]:**
1. **Betalen per resultaat.** Het verdienmodel van Werkspot is betalen per contact (AV 19.1). Overstappen naar betalen per afspraak of per getekende offerte haalt hun omzet per lead onderuit, en vraagt een offerte- en betaaltool bij de vakman die ze niet hebben. Daar komt bij dat moederbedrijf Angi onder druk staat: een afwaardering van $235 miljoen (Q2 2026), ±300 banen weg, het oude technologieplatform wordt uitgefaseerd, en de International-omzet daalde 5% "due primarily to a decrease in the number of active Pros" (Q3 2026). Dat beperkt de ruimte voor een riskante omslag van het model.
2. **De vakman is eigenaar van reviews en klanten.** Dit botst met hun lock-in (AV 11.2: na beëindiging geen toegang) en met hun anti-omzeilingsbeleid.
3. **Neutraal zijn tussen platforms.** Werkspot gaat de vakman niet helpen zijn Trustoo-, Solvari- en eigen leads te beheren, en ook niet laten zien dat Werkspot per gewonnen klus duurder is. Onze tool kan dat wel (concept 2).
4. **Lokaal vertrouwen en doorverwijzen tussen vakmannen.** Een netwerk waarin vakmannen elkaar klussen gunnen, is sociaal en lokaal. Dat koop je niet snel met een landelijk advertentiebudget.

**Risico.** Als Werkspot het maximum van 3–5 vakmannen en verificatie snel invoert, verdwijnt een deel van het verschil voor de consument. Ons blijvende verschil moet dan zitten in **het model (betalen na een waarneembare stap), het eigenaarschap van de vakman en de tools**. Daarom eerst de tool (§4).

---

## 7. Open vragen en aannames (te toetsen in interviews en pilots)

**Vakmannen**
1. Accepteren vakmannen **betalen per bevestigde afspraak** (A) als eerlijk? Welk bedrag per klusgrootte voelt redelijk? Bevestigen ze de "150 per klant"-uitspraak?
2. Wat weegt zwaarder: **voorspelbaarheid** (C) of **alleen betalen bij een opdracht** (B)? Zou een vakman in B zijn gewonnen klus eerlijk melden?
3. Hoeveel procent van hun klussen begint met een bezoek of opname, en hoeveel gaat op foto's en een indicatie?
4. Zouden ze klussen naar collega's doorverwijzen (7a), en tegen welke vergoeding?
5. Hoeveel besteden ze nu per maand aan Werkspot, Trustoo en Solvari, en hoeveel klussen levert dat op? (Validatie van concept 2; nu alleen uit reviews bekend.)

**Consumenten** *(er zijn nog geen interviews gedaan; de data komt alleen uit reviews)*
6. Is **max 3 gescreende vakmannen** genoeg keuze, of willen consumenten er meer?
7. Willen consumenten **betalen via het platform** (geldbescherming), en wat mag dat kosten? Wie betaalt de bescherming?
8. Werkt een **automatische prijsindicatie** vóór het bezoek, en schrikt een bandbreedte niet af?
9. Welk kanaal brengt consumenten met een echte klus het goedkoopst binnen (partners, lokale SEO, doorverwijzing)?

**Feiten en juridisch (uitzoeken, niet aannemen)**
10. Valt het verwerken van eigen leadmails onder AV art. 6.14 van Werkspot? Hoe zit het bij Trustoo en Solvari?
11. Vergunning en opzet voor geldbescherming of escrow: via een betaalprovider met marktplaatsfunctionaliteit, eigen stichting derdengelden, of een garantieverzekering?
12. Welke platformverplichtingen gelden voor ons als marktplaats (P2B-verordening: de ACM is sinds november 2024 bevoegd en publiceerde op 11-03-2026 een onderzoek naar platformvoorwaarden, zonder platforms bij naam te noemen (deel 1); consumentenrecht; AVG)?
13. Wat is Werkspot's huidige restitutiebeleid precies? De link in de FAQ gaf een 404 (deel 1), en het maximum aantal vakmannen per klus is niet gevonden.
14. Wat doet Klusup precies? Een consument noemt het als reden om over te stappen ("alle betalingen via Klusup"). Volgens zoekresultaten loopt betaling via het platform, met garantie en bemiddeling alleen bij betaling via Klusup. Dat is **niet zelf geverifieerd**; Klusup is nog niet in de benchmark opgenomen.

**Belangrijkste aanname om eerst te testen:** dat vakmannen een tool gebruiken en ervoor betalen *voordat* er een marktplaats is (fase 1). Klopt dat niet, dan ontbreekt de basis van de hele route en is een direct leadmodel met een groot werfbudget nodig. Dat is de route die de benchmark het minst kansrijk laat zien.
