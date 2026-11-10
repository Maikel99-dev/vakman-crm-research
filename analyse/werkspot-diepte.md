# Werkspot – diepteonderzoek (deel 1–3)

*Opgesteld 10 november 2026. Deel 4 (het concept voor een betere variant) staat in [`WERKSPOT-ALTERNATIEF.md`](../WERKSPOT-ALTERNATIEF.md). Eerdere analyse: [`werkspot.md`](werkspot.md); ruwe reviews: [`data/werkspot.csv`](../data/werkspot.csv).*

**Leeswijzer.** Alles wat niet uit een opgehaalde bron komt, staat gemarkeerd als **[aanname]** of **[interpretatie]**. Pagina's die niet op te halen waren, staan per deel onder "Niet opgehaald".

<!-- DEEL1 -->
*Deel 1 (hoe Werkspot werkt) volgt.*
<!-- /DEEL1 -->

<!-- DEEL2 -->
*Deel 2 (reviews en klachten) volgt.*
<!-- /DEEL2 -->

<!-- DEEL3 -->
## Deel 3 – Hoe anderen het doen (benchmark)

> Doel: Werkspot naast andere modellen leggen (NL en buitenland), om te zien welke ontwerpkeuzes de klachten van vakmannen verminderen of juist veroorzaken. Alle bronnen zijn op **10-11-2026** opgehaald via Apify web-fetch, tenzij anders vermeld. Wat alleen uit een zoekresultaat komt, staat als "(zoekresultaat, niet opgehaald)". Wat niet uit een bron komt, is gemarkeerd als **[aanname]**. Citaten komen alleen uit pagina's die echt zijn opgehaald. Voor Werkspot, Trustoo, Solvari en Zoofy is de basis `analyse/<slug>.md` in de repo; hier staan alleen aanvullingen.

### 3.1 Overzichtstabel

| Platform (land) | Verdienmodel (prijzen waar openbaar) | Bewaking van leadkwaliteit | Max. vakmannen per lead | Garantie voor de consument |
|---|---|---|---|---|
| **Werkspot** (NL), referentie | Per lead, €3–75. De vakman betaalt pas als de consument bij wederzijdse interesse zijn contactgegevens deelt. Volgens reviews soms ook een abonnement van ca. €70 per maand (repo: analyse/werkspot.md) | Restitutieaanvraag voor ongeldige leads, maar volgens reviews "standaard afgewezen" (repo) | Niet officieel gevonden. Reviewers noemen "5–10+" (repo) | Niet onderzocht in de repo |
| **Trustoo** (NL) | Per aanvraag (€12,50–40 volgens reviews), sinds eind 2025 plus een maandelijkse Premium-bijdrage (repo) | Reclamatie mogelijk. Wie reclameert wordt volgens reviews minder zichtbaar (repo) | 3–5 volgens reviews (repo) | Niet gevonden |
| **Solvari** (NL/BE), sinds april 2024 incl. **Offerte.nl** | Per lead (€25–30 volgens reviews), campagnes en abonnementen van €355–2.200 per maand met looptijden van 1–3 jaar, extra kosten voor "exclusieve" leads (repo) | Reclamatie met een limiet (repo) | Claimt max. 3. Vakmannen melden 7–10 belletjes per klant (repo) | Niet gevonden |
| **Zoofy** (NL) | Lidmaatschap voor onbeperkt klussen accepteren, plus marge op het tarief. De klant betaalt via Zoofy (repo) | KvK-eis en ID-verificatie. De klus gaat naar de eerste vakman die accepteert (repo) | 1 (eerste die accepteert) (repo) | Niet opgehaald |
| **Homedeal** (NL, Skydreams B.V.) | Drie vormen: *Continu* (betalen per ontvangen aanvraag), *Select* (vaste maandbundel "Reactietegoed", 1 of 12 mnd), *Pay Per Pick* (alleen betalen per zelf ontgrendelde aanvraag, geen minimale looptijd). Prijs per aanvraag "in real-time" dynamisch. Geen commissie op de omzet (AV art. 6, 7, 13) | Vergrendelde aanvraag: de vakman ziet eerst de klus en kiest dan pas of hij betaalt. Reclamatie binnen 10 dagen op vaste gronden (dubbel binnen 30 dagen, foute contactgegevens, verkeerde categorie, buiten filter, uitvoerdatum <5 dagen of >12 mnd, al vergeven ondanks contact binnen 24 uur). Creditering wel "tot een maximum" naar oordeel van Homedeal (art. 10). KvK verplicht (art. 4.3) | **Max. 6**, per categorie variabel, kan zonder bericht wijzigen (art. 5.5) | Geen. Homedeal is "geen partij" en geeft geen garanties (art. 15) |
| **Checkatrade** (UK) | Lidmaatschap: maandbedrag, je kiest postcodegebieden en "het aantal leads per jaar". Extra: print-directory en Sponsored Listings. Actie "2 maanden gratis". Prijzen staan achter "View our prices" (niet opgehaald) | "Quick ID, address & documentation check" vóór je leads krijgt. Reviews van klanten zichtbaar | Niet gevonden | **Checkatrade Guarantee: tot £1.000, 12 maanden**, als de klus via Checkatrade is geregistreerd of via Checkatrade Pay is betaald (T&C's) |
| **MyBuilder** (UK, zusje van Werkspot binnen Instapro) | Alleen een **shortlist fee** als de consument de vakman op zijn shortlist zet. "No joining fees, membership fees or any other costs." £2,50–37,50, afhankelijk van de verwachte kluswaarde. Interesse tonen is gratis. Wekelijkse factuur (FAQ, archief sept. 2023) | Telefoonnummer van elke klant geverifieerd. ID-check plus een vakbeoordeling per trade. Refund alleen in vaste gevallen (nummer werkt niet, nummer van een ander, dubbel geshortlist, direct na shortlist afgewezen). Na 24 uur zonder interesse gaat de klus naar een grotere pool. Feedback alleen van via MyBuilder geworven klanten | Niet gevonden in de FAQ | Niet gevonden |
| **Thumbtack** (VS) | Per lead, prijs varieert per klus. Direct leads worden gefactureerd zodra de klant contact opneemt (zoekresultaat en community). Pilot "booking inquiries" (alleen betalen bij een bevestigde boeking, 2–4x leadprijs) **gestopt op 18-08-2025** | **Automatische terugbetaling als de klant binnen 72 uur op geen enkele vakman reageert.** Gemaskeerde telefoonnummers per lead, gesprekken worden opgenomen (Housecall Pro-helppagina, 27-08-2026) | Niet opgehaald | Niet opgehaald |
| **Bark** (UK/int.) | Credits: **£1,80 per credit** (UK, bundels goedkoper). Prijs per lead hangt af van dienst, omvang, locatie en "customer engagement". Credits gekocht vanaf 1-11-2025 vervallen na 3 maanden. Ongebruikte credits worden niet terugbetaald (Help Centre, juni 2026) | Signalen op de lead: "Verified phone", "1st to respond", "High hiring intent", "Urgent". "Credit Back Guarantee" bij ongeldige contactgegevens of een klant die nooit iets aanvroeg. "Get Hired Guarantee" onder voorwaarden (Bark-antwoorden op Trustpilot) | Tot 5, exclusiviteit ca. +20% (zoekresultaat, **niet geverifieerd**) | Niet onderzocht |
| **Angi / Angi Leads** (VS, ex-HomeAdvisor) | Per lead plus een jaarlidmaatschap. HomeAdvisor-lidmaatschap was $287,99 per jaar (TechCrunch 2023). Leadprijzen niet officieel gepubliceerd | Sinds 2025: **de huiseigenaar kiest bij elke aanvraag welke vakmannen de lead krijgen**, met gedocumenteerde 1-op-1-toestemming. Spamfilter, slechtere leadbronnen geschrapt, creditaanvraag vereenvoudigd (CEO-brief dec. 2024) | **Van 4 naar 5.** Angi schat dat maar 7–8% van de aanvragen 5 vakmannen krijgt | Niet opgehaald |
| **Rated People** (UK) | Overgestapt op een "Unlimited leads"-abonnement in 2024 (zoekresultaat, niet opgehaald). **Merk en website in sept. 2026 overgenomen door Checkatrade Group** (Rated People-blog, opgehaald) | Niet onderzocht | Ca. 3 (zoekresultaat, niet geverifieerd) | Niet onderzocht |
| **hipages** (AU/NZ) | Abonnement met leadtegoed, bij te kopen met "boosters". In NZ in FY25 **weg van het "success fee"-model** (Stockhead, 4-11-2024) | Niet onderzocht | Niet geverifieerd (concurrent noemt 3–5) | Niet onderzocht |
| **Jobber / Housecall Pro** (VS, software) | Geen eigen leadmarkt. Abonnementssoftware met integraties: Jobber met Angi Leads, Thumbtack en Google LSA, en een Marketing Suite (reviews, campagnes, referrals). Housecall Pro met een Job Inbox voor Thumbtack, Angi Leads en Google. Leadprijzen bepaalt het leadplatform | n.v.t. Leads komen automatisch als lead of aanvraag in het systeem | n.v.t. | n.v.t. |
| **TaskRabbit / Airtasker** (commissie) | TaskRabbit: de **klant** betaalt een servicefee als percentage van het uurtarief (supportpagina). Airtasker: de Tasker betaalt een servicefee, het percentage is niet opgehaald | Betaling loopt verplicht via het platform. Airtasker houdt het geld vast tot de klus klaar is, contactgegevens pas na een geaccepteerd bod, "leaking tasks off platform" niet toegestaan | 1 (de klant kiest één Tasker) | Niet opgehaald |

### 3.2 Toelichting per platform (aanvullingen op de repo)

**Homedeal.** Dit is het enige NL-platform dat in zijn voorwaarden een vorm van "eerst zien, dan kiezen, dan betalen" vastlegt: *Pay Per Pick*, met vergrendelde aanvragen. Wel zitten er platformvriendelijke clausules in. Het maximum aantal deelnemers (≤6) kan Homedeal "op ieder moment wijzigen zonder Deelnemers hierover te informeren" (art. 5.5). Gereclameerde aanvragen worden gecrediteerd "tot een maximum welke is bepaald volgens het uitsluitende oordeel van Homedeal" (art. 10.5). Het doorverkopen of doorsturen van leads kost €500 boete per aanvraag (art. 18.1). Volgens de eigen Trustpilot-profieltekst heeft Homedeal "ruim 5.400 aangesloten vakspecialisten" en "meer dan 364.000 offerteaanvragen per jaar" (zelfrapportage). Trustpilot: 631 reviews, score 4,1, waarvan 26% 1 ster.
- Vakman, klacht: "Als specialist heb ik geprobeerd met hen samen te werken, maar ik kon geen van hun klanten bereiken en het geld werd van mijn rekening afgeschreven." (Trustpilot NL, ervaring 17-10-2026)
- Consument, over vetting: "Na controle van zijn certificaten blijkt dat hij mij valse certificaten heeft gestuurd." (Trustpilot NL, 29-10-2026). KvK-registratie zegt dus niets over vakbekwaamheid. Volgens de AV moet de deelnemer zelf zijn certificaten aantonen (art. 9.4).
- Positieve vakmanreview: niet gevonden in de 20 nieuwste reviews, die vrijwel allemaal van consumenten waren.

**Offerte.nl.** Bestaat niet meer als apart platform. offerte.nl verwijst door naar solvari.nl/offerte-overname: "In april 2024 namen we Offerte.nl over." Vakbedrijven met een Offerte.nl-overeenkomst worden naar "Solvari Pro" geleid. Voor het model, zie Solvari (repo).

**Checkatrade.** Een lidmaatschapsmodel met vetting vooraf en de bekendste consumentengarantie (£1.000). De klachten van vakmannen gaan over prijs tegenover volume. Trustpilot (1–3 sterren, nieuwste): 90.778 reviews, score 4,7, 85% 5 sterren, overwegend consumenten.
- Vakman, klacht: "Charge way to much and not enough work to share amongst 1000s of members. Really not worth the money at all. Shame because. It was an amazing company years ago." (Trustpilot UK, 06-11-2026, 1★)
- Vakman, klacht: "No jons won not many leads coming through for what we actually do but they put stuff through we dont want" (Trustpilot UK, 06-11-2026, 2★)
- Positief over de vakkant: niet gevonden (gefilterd op 1–3 sterren). Opvallend van consumentenkant: "Sent the request to 9 tradesmen, 1 provided a quote … 5 no response" (09-11-2026). Een lidmaatschap haalt de prikkel om te reageren weg.

**MyBuilder.** Inhoudelijk het Werkspot-model ("warm lead": betalen bij shortlist), maar zonder lidmaatschap en met vaste refundgronden. MyBuilder antwoordt op Trustpilot: "Rather than charging joining and ongoing membership fees as most other websites would, we charge tradespeople a relatively small fee each time they are shortlisted" (antwoord 23-10-2026). Trustpilot: 56.745 reviews, score 4,3.
- Vakman, klacht: "You are taking 100% of the financial risk while MyBuilder profits on empty introductions." (Trustpilot UK, 06-11-2026)
- Vakman, klacht: "Mybuilder does not refund my shortlist fee because the customer has replied once." (Trustpilot UK, 14-10-2026)
- MyBuilder erkent zelf nepposts: "We are aware that some non-genuine posts can appear on the platform … created by third parties" (antwoord 30-10-2026).
- Positieve vakmanreview: niet gevonden (gefilterd op 1–3 sterren).

**Thumbtack.** Het interessantste experiment voor "betalen per resultaat". In de pilot "booking inquiries" betaalden vakmannen alleen na een bevestigde boeking, tegen een hogere prijs. Thumbtack stopte de pilot op 18-08-2025: "we did find some pain points that need to be addressed in order to create an experience that consistently works well and provides a good ROI for pros … We don't have current commitments to revisit bookings" (moderator, 21-08-2025).
- Vakman, positief: "Even though we paid more per lead—and more overall—we saw higher profits because the leads were highly qualified." (Thumbtack Community, 20-08-2025)
- Vakman, klacht over het gewone model: "Before switching, we spent a significant amount of money on low-quality leads and no-shows." (zelfde post)
- Verder: automatische terugbetaling na 72 uur zonder reactie van de klant, en gemaskeerde nummers per lead (Housecall Pro-help, 27-08-2026).

**Bark.** Een creditsysteem met de prijs vooraf zichtbaar en kwaliteitssignalen op de lead. De kortere vervaltermijn van credits (3 maanden sinds 1-11-2025) en "niet terugbetaalbaar" verschuiven risico naar de vakman. Trustpilot: 112.502 reviews, score 3,8.
- Vakman, positief: "Good number of leads but disappointing that you pay for a number of leads where potential customers don't respond" (Trustpilot UK, 10-11-2026). Kort positief: "Bark it's great I got many jobs from bark" (09-11-2026).
- Vakman, klacht: "I originally signed up with their Get Hired Guarantee and when I didn't get hired … I was then told that my profile wasn't set up correctly and so I was not eligible for the refund." (Trustpilot UK, nov. 2026)

**Angi.** De belangrijkste bron is de CEO-brief (dec. 2024, archief okt. 2025). Over 2024 meldt Angi dat het aandeel aanvragen waarbij een Angi-vakman wordt ingehuurd 18% hoger lag, en dat vakmannen "27% LESS for work won" betalen. Angi definieert die take rate als "fees paid to Angi divided by the value of the jobs won and completed", gebaseerd op "pros' voluntary reports". Voor 2025: alleen leads waarbij de vakman "specifically chosen" is. Angi verwacht een hogere win rate, "as we experienced when we made a comparable change in our European business". Dat Europese bedrijf is de Instapro-groep van Werkspot en MyBuilder (repo: Werkspot "eerder Angi"), maar dat is een interpretatie. Achtergrond: in 2023 legde de FTC HomeAdvisor tot $7,2 mln aan restitutie op, omdat het de herkomst en kwaliteit van leads verkeerd had voorgesteld. Leads van affiliate-formulieren werden gepresenteerd als eigen aanvragen, en leads lagen vaak buiten vakgebied of regio. HomeAdvisor gaf geen schuld toe (TechCrunch, 23-01-2023). Citaten van vakmannen: **niet opgehaald**.

**Rated People → Checkatrade Group.** Het UK-leadplatform met een (later) abonnementsmodel is in sept. 2026 als merk en website opgegaan in Checkatrade Group (Rated People-blog: "Rated People is now part of Checkatrade Group"). Ook een Checkatrade-review van 05-11-2026 noemt dit. Dat betekent consolidatie, geen bewezen succes van het model.

**Jobber / Housecall Pro.** Ze verkopen zelf geen leads. Wel worden ze de "inbox" waarin leads van Angi, Thumbtack en Google binnenkomen. Jobber zet in op eigen lead-generatie via reviews, referrals en campagnes ("Jobber is built to grow your business sustainably over time"). hipages gaat de omgekeerde weg: van marktplaats naar software (Tradiecore, 2024).

**TaskRabbit / Airtasker.** Commissie werkt hier omdat het platform de betaling in handen heeft. Airtasker: "the Airtasker Payment Account securely holds the task funds received from the poster until you mark the task as complete", "cash payments are not supported", en contactgegevens mogen pas na een geaccepteerd bod gedeeld worden.

### 3.3 Modellen die per resultaat afrekenen – bestaan ze en werken ze?

**Ze bestaan, maar vrijwel alleen waar het platform de transactie zelf ziet of afhandelt.**

*Bewijs dat het werkt (onder voorwaarden):*
- **Platform regelt de klus en de betaling** (Zoofy, TaskRabbit, Airtasker): de "winst" is meetbaar omdat de klant via het platform betaalt. De prijs daarvan is een hoge marge en weinig vrijheid voor de vakman. Bij Zoofy: "de klant €150+ betaalt, en jij … nog geen €60-€70" (repo, Trustpilot 2026-03-12).
- **Thumbtack booking inquiries**: vakmannen waren positief, ondanks hogere kosten ("higher profits because the leads were highly qualified", 20-08-2025). Communicatie bleef in het platform tot de boeking was bevestigd. Toch gestopt, vanwege "pain points" en ROI.
- **Angi meet al per gewonnen klus** (take rate = fees / waarde van gewonnen klussen), maar rekent nog steeds per lead af. De meting leunt op vrijwillige rapportage door vakmannen.
- **Treatwell** (beauty) zou 35% commissie op de eerste boeking van een nieuwe klant rekenen en 0% op herhaalboekingen. Bron is een concurrent (Pabau), via zoekresultaat, **niet geverifieerd**.

*Bewijs dat het misgaat of wordt teruggedraaid:*
- **hipages (NZ)**: "moving away from the success fee business approach" naar een abonnement met leadtegoed (Stockhead, 04-11-2024). Een reden staat er niet bij. Een forumbron zegt "because tradies didn't like it" (zoekresultaat, niet opgehaald).
- **FixMyCar (UK, garages)**: schrapt de commissie per klus voor vaste abonnementen. CEO: "We're seeing that variable job fees do not work for auto repair businesses today. Their environment is already too challenging and too unpredictable" (AM-online, 12-10-2026).
- **Thumbtack**: de pilot is gestopt en Thumbtack heeft "no current commitments to revisit bookings" (21-08-2025).
- **MyHammer/Check24 (DE)**: de bronnen spreken elkaar tegen (provisie van 2–4% of 10–15% tegenover abonnement plus prijs per contact). Alleen derde partijen, **niet geverifieerd**.

*Fraude en omzeiling buiten het platform als structureel probleem:*
- Een succesfee prikkelt beide partijen om de deal buiten het platform te sluiten. Airtasker zegt het letterlijk: "Taking tasks off platform may seem like you're saving money on Tasker Service Fees, however it will cost you more in the long run", en sanctioneert met lagere ratings, schorsing of verbanning.
- Wat platforms ertegen doen:
  - betaling in escrow (Airtasker)
  - contactgegevens pas na acceptatie (Airtasker, MyBuilder)
  - **gemaskeerde telefoonnummers en opgenomen gesprekken** (Thumbtack)
  - geen cash
  - reviews alleen voor via het platform geworven klussen (MyBuilder verwijdert feedback als "the tradesperson was sourced outside of MyBuilder")
  - boetes op het doorsturen van leads (Homedeal: €500 per aanvraag)
- Fraude kan ook van de andere kant komen: het platform verkoopt slechtere leads dan het belooft (HomeAdvisor/FTC 2023), of nepklanten en phishing-posts (MyBuilder erkent "non-genuine posts", okt. 2026).
- **[aanname]** Bij grotere renovatieklussen gaan opname, offerte en betaling vrijwel altijd offline. Het platform ziet de "winst" dan niet en moet vertrouwen op wat de vakman meldt. Dat verklaart waarom succesfees vooral standhouden bij kleine klussen met een vaste prijs, en waarom leadplatforms terugvallen op per lead of een abonnement.

*Conclusie:* Puur "pay per win" zonder controle over communicatie en betaling is in de bronnen nergens duurzaam gebleken. Het meest belovende tussenmodel is **betalen pas na een bevestigde stap die het platform zelf kan waarnemen**: de consument kiest jou (Angi, MyBuilder, Werkspot), de afspraak is geboekt (Thumbtack-pilot), of de betaling loopt via het platform (Zoofy, Airtasker). Daarbij hoort een automatische terugbetaling als die stap niets oplevert (Thumbtack, 72 uur).

### 3.4 Lessen voor een betere variant (max. 8)

1. **Alleen betalen als de consument jou zelf kiest, en hoogstens 3–5 vakmannen per aanvraag.** Angi gaat over op "homeowners will choose the pros", maximaal 5, en verwacht een hogere win rate "as we experienced … in our European business" (CEO-brief, dec. 2024). Homedeal legt een maximum van 6 contractueel vast (AV art. 5.5).
2. **Automatische, objectieve terugbetaling zonder discussie.** Thumbtack betaalt automatisch terug als de klant binnen 72 uur op niemand reageert (Housecall Pro-help, 27-08-2026). Dat staat tegenover handmatige reclamaties met limiet of afstraffing (Solvari en Trustoo, repo) en "refund geweigerd omdat de klant één keer antwoordde" (MyBuilder-review, 14-10-2026).
3. **Eerst de klus zien, dan zelf kiezen en betalen, met de prijs vooraf zichtbaar.** Voorbeelden: Homedeal Pay Per Pick met vergrendelde aanvragen (AV art. 6.3), Bark met de creditprijs plus signalen zoals "Verified phone" en "1st to respond" (Bark Help, juni 2026), en MyBuilder ("The fee is clearly visible on the lead before you show interest", FAQ 2023).
4. **Verifieer beide kanten.** Het telefoonnummer van de consument (MyBuilder: "All customer telephone numbers go through a verification process") en de vakman op ID, adres, documenten en certificaten (Checkatrade join-pagina). Dat KvK alleen niet genoeg is, blijkt uit de Homedeal-review over valse certificaten (29-10-2026).
5. **Afrekenen per resultaat kan alleen als het platform het resultaat kan zien.** Dus betaling of boeking via het platform, gemaskeerde nummers en anti-omzeilingsregels (Airtasker-richtlijnen, Thumbtack-nummers). Zonder die controle draaien platforms het terug (hipages NZ 2024, FixMyCar 2026, Thumbtack-pilot 2025).
6. **Voorspelbare kosten zonder lock-in.** Een plafond per maand of per lead en per direct opzegbaar (Homedeal Continu en Pay Per Pick: "geen minimale looptijd", art. 13.2). FixMyCar koos voor een vast bedrag vanwege "greater certainty over customer acquisition costs" (12-10-2026). Daartegenover: de 1- tot 3-jaarscontracten van Solvari leveren de zwaarste klachten op (repo).
7. **Een consumentengarantie als vertrouwensanker, met heldere voorwaarden.** Checkatrade biedt tot £1.000 en 12 maanden (Trustpilot-profiel). Klanten klagen als een claim wordt afgewezen (review 09-11-2026). Bij Bark ontstaat hetzelfde probleem aan de vakkant met de "Get Hired Guarantee". Garanties die afketsen op kleine lettertjes kosten meer vertrouwen dan ze opleveren.
8. **Help de vakman ook aan eigen, terugkerend werk en wees de hub voor alle leadbronnen.** Jobber en Housecall Pro trekken leads van Angi, Thumbtack en Google in één inbox en zetten in op reviews en referrals (Jobber Help, 28-10-2026; Housecall Pro Help, 27-08-2026). De CEO van hipages: "60% of work is generated by word of mouth" (Stockhead, 04-11-2024).

### Bronnen

Allemaal opgehaald op 10-11-2026 via Apify web-fetch, tenzij anders vermeld.
- Homedeal Algemene voorwaarden 01-01-2026 (PDF, laatst gewijzigd 12-10-2026): https://www.homedeal.nl/companies/terms-and-conditions.pdf
- Homedeal Trustpilot NL: https://nl.trustpilot.com/review/homedeal.nl
- Offerte.nl → Solvari (gepubliceerd 08-10-2025, gewijzigd 22-09-2026): https://www.solvari.nl/offerte-overname
- Checkatrade join-pagina (gewijzigd 30-10-2026): https://join.checkatrade.com/
- Checkatrade blog/guarantee-banner: https://www.checkatrade.com/blog/
- Checkatrade Trustpilot UK (1–3★): https://uk.trustpilot.com/review/www.checkatrade.com?stars=1&stars=2&stars=3
- MyBuilder trade-FAQ (Wayback-archief 25-09-2023): https://web.archive.org/web/20230925024854/https://www.mybuilder.com/help/faq-finding-work
- MyBuilder Trustpilot UK (1–3★): https://uk.trustpilot.com/review/www.mybuilder.com?stars=1&stars=2&stars=3
- Thumbtack Community, booking inquiries (aug. 2025): https://community.thumbtack.com/discussion/1946/why-was-the-booking-inquiries-system-closed-despite-positive-feedback-from-pros-will-it-return
- Housecall Pro Help, Thumbtack-integratie (27-08-2026): https://help.housecallpro.com/en/articles/6499957-job-inbox-integration-with-thumbtack
- Bark Help, credits (bijgewerkt 10-06-2026): https://help.bark.com/hc/en-gb/articles/13346288068892-What-is-a-credit-and-how-much-does-it-cost
- Bark Help, lead pricing (bijgewerkt 08-06-2026): https://help.bark.com/hc/en-ca/articles/18043745477788-Understanding-lead-pricing
- Bark Trustpilot UK: https://uk.trustpilot.com/review/www.bark.com
- Angi CEO-brief Jeff Kip (dec. 2024, Wayback 09-10-2025): https://web.archive.org/web/20251009054329/https://intercom.help/angi/en/articles/10274582-a-note-from-angi-ceo-jeff-kip
- TechCrunch over FTC/HomeAdvisor (23-01-2023): https://techcrunch.com/2023/01/23/the-ftc-fines-homeadvisor-up-to-7-2m-for-lying-about-lead-quality-and-other-matters/
- Rated People blog ("now part of Checkatrade Group"): https://www.ratedpeople.com/blog
- Stockhead over hipages (04-11-2024): https://stockhead.com.au/news/how-hipages-plans-to-renovate-multi-billion-dollar-tradies-market/
- AM-online over FixMyCar (12-10-2026): https://www.am-online.com/news/fixmycar-scraps-per-job-garage-fees-for-subscriptions
- Jobber Help, Lead Generation (bijgewerkt 28-10-2026): https://help.getjobber.com/en/articles/lead-generation/
- TaskRabbit Service Fee: https://support.taskrabbit.com/hc/en-us/articles/46260411872155-What-s-the-Taskrabbit-Service-Fee
- Airtasker Taskers Community Guidelines (NZ): https://www.airtasker.com/nz/community-guidelines-worker/
- Repo: analyse/werkspot.md, analyse/trustoo.md, analyse/solvari.md, analyse/zoofy.md, SAMENVATTING.md §5

Alleen via zoekresultaat (WebSearch, 10-11-2026), niet opgehaald en niet gebruikt voor citaten:
- Lewis Silkin over de overname van Rated People-assets (24-09-2026)
- ratedpeople.com-blog over het Unlimited-abonnement
- Treatwell-commissie (Pabau)
- MyHammer/Check24 (clean-invoice.com, Tagesspiegel)
- Bark max. 5 vakmannen en exclusiviteit
- Checkatrade-prijzen (askbaily, whito)
- Stibbe over een werkerscoöperatie (2019)
- WRR over Zorg&Co (2017)

### Niet opgehaald

- **Werkspot: maximum aantal vakmannen per lead** staat niet in de opgehaalde FAQ (repo). Alleen reviewers noemen "5–10+".
- **Checkatrade-prijzen**: de pagina achter "View our prices" is niet gefetcht. Derde partijen spreken elkaar tegen (£30–170+/mnd).
- **MyBuilder actueel**: de huidige helppagina stuurt door naar Salesforce (support.mybuilder.com) en gaf alleen "Loading". Daarom is het archief van sept. 2023 gebruikt. Huidige prijzen dus mogelijk anders.
- **Thumbtack-helpcentrum** (refundbeleid): https://help.thumbtack.com/article/how-to-request-a-refund gaf een lege pagina (JavaScript). De 72-uursregel komt daarom uit Housecall Pro-documentatie.
- **Angi**: de live CEO-pagina gaf 404, daarom de Wayback-versie. Citaten van vakmannen over Angi en een bevestiging van "Angi Services" met vaste prijs zijn niet gevonden.
- **Trustpilot-citaten van vakmannen** voor Thumbtack, Angi, Rated People, hipages, TaskRabbit en Airtasker zijn niet opgehaald (zuinigheid). Positieve vakmanreviews voor Checkatrade en MyBuilder zijn niet gezien, omdat op 1–3 sterren is gefilterd.
- **Airtasker-feepercentages** (bronnen spreken elkaar tegen: 7,5–20%) en de **TaskRabbit-clausule tegen betalen buiten het platform** zijn niet in officiële bronnen opgehaald.
- **Coöperaties van vakmannen** met een eigen klussenplatform: geen bestaand NL-voorbeeld gevonden. Alleen een juridische analyse (Stibbe, 2019) en een zorgcoöperatie (WRR, 2017), beide via zoekresultaat.
- **Consumentengarantie** van Werkspot, Trustoo, Solvari, Zoofy, MyBuilder, Thumbtack en Angi is niet onderzocht of opgehaald.
- **Houzz Pro, Porch, Networx en Yelp**: alleen zoekresultaten (abonnement of per lead, prijzen tegenstrijdig). Niet opgenomen in de tabel.

<!-- /DEEL3 -->
