# Werkspot – diepteonderzoek (deel 1–3)

*Opgesteld 10 november 2026. Deel 4 (het concept voor een betere variant) staat in [`WERKSPOT-ALTERNATIEF.md`](../WERKSPOT-ALTERNATIEF.md). Eerdere analyse: [`werkspot.md`](werkspot.md); ruwe reviews: [`data/werkspot.csv`](../data/werkspot.csv).*

**Leeswijzer.** Alles wat niet uit een opgehaalde bron komt, staat gemarkeerd als **[aanname]** of **[interpretatie]**. Pagina's die niet op te halen waren, staan per deel onder "Niet opgehaald".

<!-- DEEL1 -->
## Deel 1 – Hoe Werkspot werkt

> Alle pagina's opgehaald op **10-11-2026** via Apify web-fetch, tenzij anders vermeld. Citaten staan letterlijk tussen aanhalingstekens. Eigen duiding is gemarkeerd als **[interpretatie]**, ontbrekende onderbouwing als **[aanname]**.
>
> **Belangrijke bronnoot over datums.** Alle opgehaalde blogpagina's van werkspot.nl tonen "Bijgewerkt op 24-08-2026" en hebben in de metadata `datePublished` 2026-08-24 (11:53–11:56 uur). Dat geldt ook voor een actie uit juni 2017 (cashback-blog) en voor twee FAQ-pagina's die elkaar tegenspreken (€3–€60 en €3–€75). **[interpretatie]** 24-08-2026 is dus een migratie- of herpublicatiedatum van het CMS en geen inhoudsdatum. De bewering in de repo dat de €3–€75 "per de FAQ van 24-08-2026" geldt, klopt letterlijk, maar zegt niets over wanneer die prijsband is ingegaan.

### 1. Eigenaar en structuur

| Feit | Bron |
|---|---|
| Juridische entiteit: "Werkspot BV, gevestigd te Tilburg en kantoorhoudende aan de (1017 BS) Herengracht 469 te Amsterdam, KvK nummer: 18079951" | AV vakmensen art. 1.15 (versie "Amsterdam, maart 2026") |
| Opgericht in 2005 door Joost Gielen en Sjoerd Eikenaar. Sinds 2013 "onderdeel van … HomeAdvisor", dat volgens deze pagina "deel uit[maakt] van IAC" | werkspot.nl/over-ons (opgehaald 10-11-2026). **Let op: deze pagina is verouderd**, zie hieronder |
| "Vanuit Amsterdam werken 120 internationale professionals aan het succes van onze merken Werkspot en Instapro" | werkspot.nl/over-ons |
| **IAC heeft Angi op 31 maart 2025 afgesplitst.** "IAC no longer owns any shares of Angi capital stock"; Angi is "an independent, publicly traded company". Joey Levin werd Executive Chairman van Angi, en Jeff Kip was toen CEO. | IAC/Angi-persbericht, 1 april 2025 (SEC 8-K ex. 99.1) |
| Angi (10-K over 2025): "We also own and operate the following international businesses … (i) HomeStars, MyBuilder, MyHammer, Travaux and Werkspot, leading home services marketplaces in Canada, the United Kingdom, Germany, France and the Netherlands, respectively, (ii) the Austrian operations of MyHammer and (iii) the Italian operations of Werkspot." | Angi 10-K FY2025 (ingediend 20-02-2026) |
| Segmenten: "(i) U.S. and (ii) International (consisting of businesses in Europe and Canada)". "International revenue primarily comprises leads revenue for consumer matches and membership subscription revenue from Pros." | Angi 10-K FY2025 |
| International-omzet: $126,5 mln in 2025 tegen $129,0 mln in 2024 (−2%), dat is 12% van de totale Angi-omzet ($1.030,5 mln). Oorzaak volgens Angi: "a management decision to change the business model of the Canadian business when migrating it onto the European platform" | Angi 10-K FY2025 |
| Q3 2026: International-omzet $30,9 mln (−5% j-o-j) "due primarily to a decrease in the number of active Pros as well as unfavorable foreign currency exchange rate movements". International Adjusted EBITDA $10,3 mln (Q3 2025: $8,6 mln). De vaste kosten van International daalden van 35% naar 21% van de omzet. | Angi Q3 2026-persbericht, 03-11-2026 (SEC 8-K) |
| Angi in 2026: nieuwe CEO **Mike Steib** ("My first 45 days…"). In Q2 2026 een afwaardering van goodwill en immateriële activa van $235,2 mln. Op 03-11-2026 een aangekondigde reductie van "approximately 300 roles" wereldwijd. Een "planned retirement of our legacy technology platform". | Angi Q3 2026-persbericht |
| Zustermerken die de over-ons-pagina noemt: MyBuilder (UK), Travaux.com (FR), My-Hammer.de (DE). In Italië: "nummer drie in de markt met 60.000 klussen per jaar en ruim 11.000 aangesloten vakmensen" (verouderde tekst) | werkspot.nl/over-ons |

**Wat er 2024–2026 gebeurde, samengevat.** IAC heeft Angi per 31-03-2025 volledig afgestoten. Werkspot is sindsdien een dochter van het zelfstandige, beursgenoteerde Angi Inc. en valt binnen het segment "International". In de opgehaalde bronnen (10-K FY2025, Q3 2026-persbericht) staat geen aankondiging van verkoop of afsplitsing van de internationale tak. **[interpretatie]** Wel zijn er signalen van druk bij de moeder: omzetdaling, een goodwill-afwaardering, een nieuwe CEO, ontslagen en een migratie naar één "European platform". Of Werkspot daardoor verandert, blijkt niet uit de bronnen.
- In de 10-K wordt Italië aangeduid als "the Italian operations of Werkspot". De Instapro-merknaam staat er niet in, maar de over-ons-pagina noemt nog wel "onze merken Werkspot en Instapro". StarOfService komt in geen enkele opgehaalde bron voor. **[aanname]** Het hoort niet bij deze groep.
- De over-ons-pagina is aantoonbaar verouderd: ze noemt HomeAdvisor/IAC als moeder en Tinder/Vimeo als zusterbedrijven. Gebruik haar niet als bron voor de huidige eigendomsstructuur.

### 2. Verdienmodel voor vakmannen

**Inschrijven.** Inschrijven is gratis ("Schrijf je gratis in"; "Vakmensen kunnen gratis lid worden"). Bron: werkspot.nl/vakman/registreren en de homepage.

**Leadprijs: wat en wanneer.**
- Definitie: "Leadprijs: de door de Vakman verschuldigde vergoeding wanneer de Contactgegevens van de Klant met de Vakman worden gedeeld na een Reactie." (AV art. 1.8)
- "De Leadprijs wordt verschuldigd wanneer de Contactgegevens van de Klant na een Reactie met de Vakman worden gedeeld. Het is niet nodig dat de Vakman de opdracht krijgt toegewezen om de Leadprijs verschuldigd te laten zijn." (AV art. 19.1)
- Registratiepagina: "Reageer op zoveel opdrachten als je wilt. Op basis van je profiel, eerdere opdrachten en reviews beslissen opdrachtgevers met wie ze hun contactgegevens willen delen." En: "Wanneer een opdrachtgever contactgegevens met jou deelt, brengen wij je leadkosten in rekening."
- AV opdrachtgevers art. 3.2 noemt twee varianten: "Afhankelijk van de beschikbare functionaliteit kan een Vakman de Contactgegevens van de Klant onmiddellijk na het reageren op een Advertentie verkrijgen, of kan hij een Reactie indienen waarvoor bevestiging door de Klant nodig is voordat Contactgegevens worden gedeeld." **[interpretatie]** Er bestaat dus naast het gebruikelijke model van wederzijdse interesse ook een directe variant, waarbij de vakman meteen betaalt.
- Een lead bevat "een naam, e-mailadres en een telefoonnummer" (FAQ).

**Hoogte en bepaling van de leadprijs.**
- FAQ "brandende vragen": "De leadprijs is variabel en onder andere gebaseerd op vakgebied, oppervlakte, de hoeveelheid (denk hierbij aan deuren, kozijnen, wanden en/of trappen) en het materiaal. De leadprijs staat altijd vermeld voordat je op een opdracht reageert en kan variëren van € 3,00 tot € 75,00. Deze prijs staat vast en zal nooit worden aangepast nadat je hebt gereageerd." (werkspot.nl/blog/faq-brandende-vragen-over-werkspot, "Bijgewerkt op 24-08-2026") **→ bevestigd.**
- **Tegenstrijdigheid:** werkspot.nl/blog/faq (ook "Bijgewerkt op 24-08-2026") noemt woordelijk dezelfde tekst, maar met "**€ 3,00 tot € 60,00**". **[interpretatie]** De maximumprijs is ooit verhoogd van €60 naar €75, maar wanneer is niet vast te stellen.
- AV art. 19.1: de leadprijs "is afhankelijk van de inhoud van de gevraagde kluswerkzaamheden en de wijze waarop de Reactie wordt verzonden en kan van tijd tot tijd wijzigen. Het bedrag van de Leadprijs wordt aan de Vakman meegedeeld voordat hij een Reactie verzendt…"
- AV art. 19.7 (slot): "Het voorgaande geldt niet voor de Leadprijs. Deze kan te allen tijde en zonder nadere aankondiging door Werkspot gewijzigd worden."
- Werkspot zelf in de FAQ: "Het platform is zo ontworpen dat de inkomsten uit de opdrachten die je mag uitvoeren, na verloop van tijd al jouw leadkosten dekken. Dat geldt dus ook voor de kosten die je hebt gemaakt voor de leads die niet succesvol zijn."
- Alle prijzen zijn exclusief btw (AV art. 19.5).

**Abonnementen, pakketten en gesponsorde plaatsing.**
- De AV noemen "abonnementen en pakketten" (art. 1.10) en een "maandelijkse of anderszins periodiek verschuldigde vergoeding" naast de leadprijs, "bij vooruitbetaling" (art. 19.6). Die vergoeding is gekoppeld aan overeenkomsten voor bepaalde duur onder art. 18, die gelden voor overeenkomsten "aangegaan voor 1 april 2018".
- Gesponsorde plaatsing: "Vakmannen hebben de mogelijkheid om Werkspot een extra maandelijks bedrag te betalen voor gesponsorde plaatsing, waarbij hun Profielpagina (bij toerbeurt met andere gesponsorde Vakmannen) op een prominente positie boven profielen … kan worden weergegeven. Alle gesponsorde plaatsingen zijn onderworpen aan afzonderlijke algemene voorwaarden." (art. 6.8)
- **Historische prijs:** een actie uit juni 2017 noemt "de waarde van het basis abonnement van €240,-" (werkspot.nl/blog/cashback-zomeractie…). Die actie liep "tot en met 30 juni 2017"; het is onduidelijk of €240 een maand-, kwartaal- of jaarbedrag was.
- **Huidige abonnementsprijzen en de prijs van gesponsorde plaatsing zijn niet gevonden** op openbare pagina's. Reviewers in de repo noemen "ongeveer 70 euro" per maand (zie analyse/werkspot.md). Dat is niet geverifieerd.
- Credits: "Werkspot kan, maar is onder geen enkele omstandigheid verplicht om, aan de Vakman Credits ter beschikking te stellen." (art. 19.3)

**Facturatie en incasso.**
- FAQ: "Maandelijks wordt op de eerste van de maand gefactureerd."
- AV art. 20.1: de leadprijs wordt gefactureerd "in de maand volgend op de maand waarin de Vakman de Lead heeft ontvangen, of eerder, als de Vakman de kredietlimiet op zijn Account heeft overschreden."
- Art. 20.2: automatische incasso. Art. 20.3: bij niet-betaling volgt blokkade van het account. Art. 20.4: incassokosten "minimaal 15% van de hoofdsom, met een minimumbedrag van EUR 100,-". Art. 20.7: "Enig beroep door de Vakman op opschorting, verrekening of aftrek is niet toegestaan."

**Hoeveel vakmannen per lead of klus?**
- **Geen maximum gevonden** in de AV of op de opgehaalde pagina's. Consumentenpagina: "dan introduceren we je bij meerdere gekwalificeerde vakmannen" (werkspot.nl/hoe-werkt-het). Registratiepagina: "Reageer op zoveel opdrachten als je wilt."
- Directe aanvraag (selectie door de consument): "De selectie is beperkt exclusief, de termijn hiervoor staat altijd bij de opdracht aangegeven. Ontvangt een opdracht binnen deze termijn te weinig reacties, dan wordt deze naar andere vakmannen gestuurd." En: "Ontvang je hierop een antwoord met telefoonnummer van de klant? Dan betaal je de lead. Ontvang je niets? Dan betaal je ook niets!" (werkspot.nl/blog/nieuw-bij-werkspot-directe-aanvraag; inhoudsdatum onbekend)
- Reviewers melden 5–10+ vakmannen per lead (zie analyse/werkspot.md). Dat is niet door Werkspot bevestigd.

**Rangschikking (bepaalt wie de consument ziet), AV art. 6.6.** De parameters "in volgorde van typisch belang":
1. relevantie (vakgebied);
2. geografische nabijheid;
3. klantfeedback ("Hoe beter uw beoordeling, hoe hoger…");
4. interacties: "Wij beoordelen daarom hoeveel antwoorden u in de week vóór het aanmaken van de Advertentie door de Klant hebt verzonden en of deze antwoorden betrekking hadden op vergelijkbare Advertenties. Hoe hoger het aantal antwoorden, hoe hoger u in de rangschikking voor de Klant verschijnt.";
5. willekeur: een boost voor vakmannen die "2 maanden of minder actief" zijn.

**[interpretatie]** Wie meer reageert, en dus meer leadkosten kan oplopen, wordt hoger getoond.

**Restitutie.**
- AV art. 19.2: "Werkspot hanteert een restitutiebeleid, waaronder de Vakman onder omstandigheden een restitutie kan aanvragen van de Leadprijs … De Restitutie wordt uitgekeerd in de vorm van een tegoed ter hoogte van de Leadprijs, welke uitsluitend gebruikt kan worden op het Platform. Een Restitutie wordt enkel toegekend onder de omstandigheden die omschreven zijn in het restitutiebeleid en Werkspot bepaalt geheel naar eigen inzicht of daar in een concreet geval sprake is."
- AV art. 19.4: "Restituties en Credits zijn geldig voor de duur van 1 (een) jaar, tenzij anders overeengekomen. Bij het einde van de Overeenkomst, op welke grond dan ook, komen alle Restituties en Credits te vervallen. Restituties en Credits worden niet in geld uitgekeerd."
- FAQ, bij een onbereikbare klant: "houd rekening met ongeveer een week. Klopt de contactinformatie niet? Dan kan je met ons contact opnemen". Die link (werkspot.nl/blog/leads-en-restitutie) geeft een **404**.
- **Het restitutiebeleid zelf (geldige gronden, aanvraagtermijn) is niet gevonden.** Zie "Niet opgehaald".

**Contractduur en opzegging.**
- Standaard geldt onbepaalde duur (art. 17.1). Opzeggen: "op ieder moment … door een e-mail te sturen naar info@werkspot.nl met het onderwerp 'Verwijdering Account'", of via een opzegproces in het account als dat er is (art. 17.2). Werkspot zelf kan opzeggen met "een opzegtermijn van één maand" (art. 17.3).
- Oude jaarcontracten (aangegaan vóór 1 april 2018): duur 1 jaar met stilzwijgende verlenging met 1 jaar (art. 18.2). Opzeggen kan alleen online via "Mijn Account"; "Opzeggingen via telefoon, post of e-mail worden in verband met fraudegevoeligheid niet in behandeling genomen" (art. 18.3).
- Tariefwijziging: periodieke bedragen gaan "1 (één) maand na bekendmaking" in. De vakman kan opzeggen "gedurende 14 (veertien) dagen voorafgaand aan de datum waarop de wijziging van kracht wordt" (art. 19.7). Daarnaast mag Werkspot jaarlijks indexeren volgens het CBS-cijfer, zonder opzegrecht (art. 19.8).

### 3. Klantreis consument

1. **Klus plaatsen, gratis.** "Het is makkelijk, gratis en vrijblijvend." "Vermeld zoveel mogelijk informatie… Tip: Neem foto's met je telefoon" (werkspot.nl/hoe-werkt-het). De homepage zegt: "Plaats je klus gratis".
2. **Reacties ontvangen.** "Nadat je je klus geplaatst hebt, sturen we je aanvraag door naar gekwalificeerde vakmannen. Wacht rustig totdat je voorstellen ontvangt via de e-mail." Een voorstel bestaat uit een persoonlijk bericht en, "wanneer mogelijk", een "richtprijs" (hoe-werkt-het). Er is ook een consumentenapp met "notificaties en de chatfunctie" (homepage).
3. **Directe aanvraag.** De consument "ontvangt een lijst met aanbevolen vakmannen" en kan zelf vakmannen selecteren (blog directe aanvraag).
4. **Contactgegevens delen.** De consument beslist met wie hij contactgegevens deelt; pas dan betaalt de vakman (registratiepagina; AV art. 1.8/19.1). In sommige functionaliteit krijgt de vakman de gegevens direct (AV opdrachtgevers art. 3.2).
5. **Afspraak en uitvoering.** De overeenkomst komt pas tot stand op het moment dat de opdrachtgever "dit uitdrukkelijk aan de Vakman heeft bevestigd. Werkspot is bij Overeenkomsten tussen de Opdrachtgever en de Vakman geen partij." (AV opdrachtgevers art. 5.8; vakmensen art. 6.12)
6. **Review.** Een review kan alleen als "het werk reeds is begonnen of je een aanbetaling hebt gedaan", maximaal 1000 tekens, met een score van 1–5 sterren. Het profielgemiddelde is "het gemiddelde van hun gecombineerde beoordelingen" (werkspot.nl/voorwaarden-voor-reviews, "Updated: 17 Januari 2025").
7. **Kosten voor de consument:** geen. Het platform is "gratis en vrijblijvend"; consumenten betalen geen bemiddelingskosten volgens de opgehaalde pagina's.
8. **Garantie: niet gevonden.** Er is geen "Werkspot Garantie" op de opgehaalde pagina's. Bij ontevredenheid verwijst Werkspot naar eigen stappen tegenover de vakman: melden, ingebrekestelling, branchevereniging of Juridisch Loket. Het platform zegt alleen "Bij twijfel neem dan contact met ons op" (werkspot.nl/blog/niet-tevreden-over-het-werk-van-de-vakman). Volgens de AV heeft Werkspot "slechts een faciliterende rol" (opdrachtgevers art. 3.2).
   - **[interpretatie]** Dit is een duidelijk verschil met Angi in de VS. Daar noemt het Q3-persbericht een "service guarantee expense" als kostenpost (die gaat over het Amerikaanse en geconsolideerde bedrijf, niet specifiek over Werkspot).

### 4. Aantallen van de eigen site (opgehaald 10-11-2026)

| Cijfer | Waar | Opmerking |
|---|---|---|
| **42.491 vakmensen**, **25+ vakgebieden**, **843.038 reviews** | homepage werkspot.nl | Live teller (cache-leeftijd ±18 min) |
| 42.448 vakmannen, **6.765.869 klussen**, 842.869 reviews | werkspot.nl/over-ons | Zelfde teller, cache ±14,6 uur oud |
| "Meer dan een half miljoen echte reviews" | homepage | |
| 16.475 dakdekkers, 8.135 bouwbedrijven, 14.293 badkamerinstallateurs "in Nederland" | homepage | **[interpretatie]** De categorieën overlappen: de som is groter dan de helft van het totaal, dus vakmannen staan in meerdere categorieën |
| "45.000 geplaatste opdrachten per maand" | blog "frisse nieuwe look" | Inhoudsdatum onbekend (datum 24-08-2026 is CMS-datum) |
| "meer dan 350.000 klussen" per jaar, "meer dan 8.500 aangesloten vakmensen" | over-ons (lopende tekst) | **Verouderd** (vgl. de teller van 42.448). Niet gebruiken als actueel cijfer |
| "Rob 4.9/5" | homepage, registratiepagina | Betekenis onduidelijk (testimonial of score?). **Geen gemiddelde platformscore gevonden** |

**[interpretatie]** Volgens de 10-K haalt International zijn omzet uit lead fees en abonnementen. Q3 2026 noemt "a decrease in the number of active Pros". "42.491 vakmensen" is waarschijnlijk het aantal geregistreerde profielen, niet het aantal actieve betalende vakmannen **[aanname]**.

### 5. Recente wijzigingen 2024–2026

| Datum | Wijziging | Bron |
|---|---|---|
| 17-01-2025 | Nieuwe "Voorwaarden voor Reviews"; reviews van vóór die datum "vallen onder onze vorige richtlijnen" | werkspot.nl/voorwaarden-voor-reviews |
| 31-03-2025 | IAC splitst Angi af; Werkspot valt onder het zelfstandige Angi Inc. | persbericht 01-04-2025 |
| 2025 | Canadese tak (HomeStars) gemigreerd naar "the European platform" | Angi 10-K FY2025 |
| dec. 2024 → mrt. 2026 | **Nieuwe AV-versie** ("Amsterdam, maart 2026"). De archiefversie van 11-08-2025 heet "Amsterdam, December 2024". Nieuw in maart 2026 (niet aangetroffen in de versie van december 2024, gecontroleerd op trefwoorden): art. 6.10 (geen omzeiling van de leadprijs via contactgegevens, leadprijs niet als toeslag), **art. 6.14 (verbod op bots/scrapers/databases)**, art. 7.5–7.6 (geen beïnvloeding van reviews), art. 9.6A/B (één account, geen herregistratie), definities voor DSA-begrippen (Illegale inhoud, Besluit, Verificatiegegevens, Gesponsorde plaatsing), art. 6.8 (gesponsorde plaatsing). Art. 19.1 kreeg de zin "Het is niet nodig dat de Vakman de opdracht krijgt toegewezen…" | werkspot.nl/algemene-voorwaarden (actueel) vs web.archive.org-snapshot 20250811 |
| onbekend (≤ 2026) | Maximale leadprijs van €60 naar €75 (twee FAQ-pagina's naast elkaar) | werkspot.nl/blog/faq vs /blog/faq-brandende-vragen-over-werkspot |
| onbekend | Nieuwe huisstijl ("frisse nieuwe look"). De asset-paden van de registratiepagina bevatten "rebrand" | blog; registratiepagina |
| Q1 2026 | Reorganisatie bij Angi; in Q2 2026 afwaarderingen van $235,2 mln | Angi Q3 2026-persbericht |
| 03-11-2026 | Angi schrapt ±300 functies wereldwijd; nieuwe CEO Mike Steib; legacy-techplatform wordt uitgefaseerd | Angi Q3 2026-persbericht |

- **Nederlandse pers (Emerce, Sprout/MT, FD, Tweakers, NOS, Kassa, Radar):** via WebSearch is **geen** artikel uit 2024–2026 specifiek over Werkspot gevonden.
- Kassa heeft alleen een forumbijdrage van een gebruiker uit **05-04-2019**, waarin leadprijzen van "variërend 5,- tot 20,-" worden genoemd (bnnvara.nl/kassa/vraag-beantwoord/…/werkspot). Die is alleen als historisch referentiepunt bruikbaar.
- ACM: geen Werkspot-specifiek besluit gevonden. De ACM is sinds november 2024 bevoegd voor de P2B-verordening en publiceerde op 11-03-2026 een onderzoek naar de ervaringen van zakelijke gebruikers met de AV van platforms (acm.nl, gerelateerde publicaties; platforms worden op de opgehaalde pagina niet genoemd).
- **[interpretatie]** De nieuwe AV van maart 2026 vallen in tijd samen met de P2B-/DSA-handhaving. Een oorzakelijk verband is niet aangetoond.

### 6. Algemene voorwaarden – letterlijke artikelen

Bron: https://www.werkspot.nl/algemene-voorwaarden, sectie "Voor Vakmensen", ondertekend "**Amsterdam, maart 2026**" (opgehaald 10-11-2026). De opdrachtgeversectie is eveneens ondertekend met "Amsterdam, maart 2026".

**6a. Automatisch verwerken, scrapen en doorsturen van leads/gegevens**
- **Art. 6.14:** "De Vakman mag geen bots, scrapers of andere geautomatiseerde middelen gebruiken om toegang te krijgen tot het Platform of gegevens daarvan te verzamelen, noch databases opbouwen uit Platformgegevens, behalve waar dit uitdrukkelijk schriftelijk door Werkspot is toegestaan."
- **Art. 10.2:** "Het is de Vakman niet toegestaan het Platform of enige inhoud daarvan, zonder schriftelijke toestemming van Werkspot, op welke wijze dan ook aan derden ter beschikking te stellen, te reproduceren, verspreiden, verzenden, of op welke wijze dan ook in een ander document of ander materiaal te verwerken. Dit houdt onder meer in dat het Vakman niet is toegestaan, zonder voorafgaande schriftelijke toestemming van Werkspot, een substantieel gedeelte van de inhoud van (een) databank(en) op te vragen en te hergebruiken en/of nietsubstantiële gedeelten van de inhoud van een databank(en) herhaald en systematisch op te vragen en te hergebruiken in de zin van de Databankenwet."
- **Art. 6.13:** "Het gebruik van de persoonsgegevens die door middel van het Platform door de Vakman worden verkregen mogen uitsluitend worden gebruikt voor het doel waarvoor deze zijn verstrekt. Het is niet toegestaan om deze gegevens te verwerken voor enig ander doel, waaronder begrepen – maar niet daartoe beperkt – iedere vorm van ongevraagde communicatie (spam). Het is evenmin toegestaan om persoonsgegevens (waaronder e-mail adressen) van Gebruikers te verzamelen voor welk doel dan ook. Schending van dit artikel 6.11 is een wezenlijke tekortkoming en kan leiden tot onmiddellijke beperking, opschorting of beëindiging." (*Let op: de tekst van 6.13 verwijst zelf naar "artikel 6.11"; dat is een nummeringsfout in de bron.*)
- **Art. 9.6** (accounttoegang): "De Vakman mag uitsluitend zijn werknemers of gemachtigde vertegenwoordigers toegang verlenen tot het Account voor legitieme zakelijke doeleinden in verband met het gebruik van de Diensten, mits de Vakman volledig verantwoordelijk blijft voor alle handelingen en nalatigheden die via het Account door die personen worden verricht."
- [interpretatie, niet juridisch getoetst]
  - Een CRM dat inlogt op het Werkspot-account en daar automatisch gegevens ophaalt, valt onder de letterlijke tekst van 6.14 ("bots, scrapers of andere geautomatiseerde middelen … toegang te krijgen tot het Platform"), tenzij Werkspot schriftelijk toestemming geeft.
  - Of het automatisch verwerken van notificatiemails die de vakman zelf ontvangt hieronder valt, staat niet expliciet in de tekst. 6.13 staat gebruik van verkregen persoonsgegevens toe "voor het doel waarvoor deze zijn verstrekt"; de aanname is dat dat het opvolgen van de klus is.
  - "databases opbouwen uit Platformgegevens" (6.14) en 10.2 kunnen ook een klantdossier raken dat uit platformgegevens is opgebouwd. Hier is juridisch advies nodig.

**6b. Contact met de klant buiten het platform; gebruik van contactgegevens**
- **Art. 1.16:** Contactgegevens worden gedeeld "om directe communicatie op of buiten het Platform mogelijk te maken". **[interpretatie]** Contact buiten het platform is dus uitdrukkelijk voorzien zodra de gegevens gedeeld zijn.
- **Art. 6.10:** "De Vakman mag geen Contactgegevens of andere identificatoren opvragen, publiceren of uitwisselen met het doel of effect de Leadprijs te ontwijken, onder meer door dergelijke gegevens te plaatsen in berichttekst, afbeeldingen, bijlagen of profielvelden die niet voor Contactgegevens zijn bedoeld. De Vakman mag de Leadprijs niet als afzonderlijke toeslag aan de Klant presenteren of stellen dat de Klant verplicht is deze te vergoeden. Dit belet de Vakman niet om zijn algehele prijsstelling zelfstandig vast te stellen."
- **Art. 6.15:** "Indien de Vakman in strijd handelt met het in artikel 6.10 bepaalde verbeurt hij, zonder nadere waarschuwing of ingebrekestelling en zonder dat daartoe rechterlijke tussenkomst is vereist, een direct opeisbare boete van EUR 1.000 (duizend euro) per gebeurtenis, waarbij het gebruik van een persoonsgegeven geldt als één gebeurtenis…"
- **Art. 6.4:** "Vakman zal slechts berichten plaatsen op en versturen via het Platform met als doel het verkrijgen van een opdracht … en zal zich onthouden van het versturen van ongewenste en/of ongevraagde berichten aan Opdrachtgevers."
- **Art. 6.9 sub e:** verboden is "materiaal waarin op enige wijze melding wordt gemaakt dan wel wordt verwezen naar een andere, met de Dienst of het Platform concurrerende of vergelijkbare dienst, website of platform".
- **Art. 11.1 sub h:** uitsluiting is mogelijk als "de Vakman de betaling van de Leadprijs op enige wijze tracht te omzeilen".
- **Huisregels** (werkspot.nl/kwaliteitseisen, onderdeel van de AV via art. 6.2 sub g): "gebruik geen waarschuwingen over kosten die voor jou verbonden zijn aan een reactie van de consument."
  - **[interpretatie]** Dit verklaart waarom vakmannen in reviews klagen dat de consument niet weet dat reageren geld kost: de vakman mag dat in zijn bericht niet zeggen.
- **Consumentenkant, art. 5.9 opdrachtgevers:** voor de opdrachtgever geldt dezelfde beperking op het gebruik van persoonsgegevens van gebruikers.

**6c. Reviews (eigendom, verwijderen)**
- **Art. 10.1:** "Alle intellectuele eigendomsrechten met betrekking tot het Platform behoren bij uitsluiting toe aan Werkspot en/of haar licentiegevers, met uitzondering van het materiaal dat door de Gebruikers is aangeleverd door het plaatsen van Reacties, Advertenties, opdrachten, reviews, voorstellen of anderszins. Door inhoud te uploaden … verleent de Vakman aan Werkspot een niet-exclusieve, wereldwijde, royaltyvrije licentie voor de duur van de Overeenkomst … Behoudens de in dit Artikel verleende licentie blijven alle rechten op door de Vakman verstrekte inhoud bij de Vakman of diens licentiegevers."
- **Art. 7.2:** "De inhoud van een review wordt bepaald door de Opdrachtgever. Werkspot heeft daar geen invloed op en kan niet verantwoordelijk worden gehouden voor de inhoud van reviews."
- **Art. 7.3:** "Werkspot is te allen tijde gerechtigd een review te verwijderen. Zij kan daar mede, doch niet uitsluitend, toe overgaan indien naar aanleiding van een melding blijkt dat de review onjuist, onbetrouwbaar of onmiskenbaar onrechtmatig is…"
- **Art. 7.5:** "De Vakman mag niet trachten een Klant te beïnvloeden, onder druk te zetten of te bewegen een beoordeling te wijzigen of te verwijderen door restituties, kortingen of andere voordelen aan te bieden waarop de Klant niet wettelijk recht heeft. Schending kan leiden tot opschorting of beëindiging van het Account."
- **Art. 7.6:** "De Vakman mag geen beloningen aanbieden voor positieve beoordelingen, verwijderingsverzoeken als voorwaarde voor het oplossen van een geschil of anderszins het beoordelingsproces manipuleren."
- **Art. 11.2 (slot):** "De Vakman zal na beëindiging van de Dienst geen technische en/of contractuele toegang meer hebben tot de door de Vakman verstrekte of gegenereerde informatie."
- **Reviewbeleid (17-01-2025):**
  - "Vakmensen hebben ook het recht om bezwaar te maken tegen een beoordeling die over hen is achtergelaten. We zullen alle ontvangen bezwaren onderzoeken en wanneer we van mening zijn dat een beoordeling in strijd is met onze algemene voorwaarden of dit beleid, kunnen we de beoordeling." (zin onaf in de bron)
  - "We accepteren ook beoordelingen voor vakmensen van maximaal vijf klanten van buiten ons platform … De beoordeling wordt pas gepubliceerd als de factuur is ontvangen."
  - "We bepalen naar eigen oordeel of we een beoordeling op verzoek verwijderen of niet."
- **[interpretatie]**
  - De review is geen eigendom van de vakman: die is geschreven door de opdrachtgever.
  - De AV bevatten geen recht om reviews te exporteren of mee te nemen.
  - Na beëindiging verliest de vakman de toegang (11.2).
  - Dit bevestigt de lock-in-klacht in analyse/werkspot.md.

**6d. Accountblokkade en beëindiging**
- **Art. 9.2:** als aanvullende informatie niet binnen 14 dagen wordt verstrekt, mag Werkspot "het Account te blokkeren totdat de gevraagde informatie verstrekt is."
- **Art. 9.4**, gegronde redenen om te weigeren of te verwijderen: "(i) de Vakman voldoet niet aan de kwaliteitscriteria …, (ii) het bestaan van een vermoeden dat de Vakman in strijd handelt met de Overeenkomst …, (iii) … eerder misbruik …, (iv) de Vakman heeft negatieve beoordelingen en/of klachten van Opdrachtgevers ontvangen en het blokkeren is noodzakelijk om de belangen van de andere Gebruikers te beschermen, (v) … niet langer de juiste kwalificaties …, (vi) de Vakman heeft een onbetaalde factuur, (vii) de Vakman veroorzaakt substantiële schade aan Opdrachtgevers, (viii) enige andere niet nader gespecificeerde reden die door Werkspot op het moment van beoordeling als belangrijk wordt geacht."
- **Art. 9.5:** bij beperking of opschorting krijgt de vakman "een motivering van dat Besluit op een duurzame gegevensdrager", en kan hij het besluit "aanvechten via het interne klachtenafhandelingssysteem".
- **Art. 9.6B:** "Indien een Account om gegronde redenen wordt beëindigd, mag de Vakman zich niet opnieuw registreren zonder voorafgaande schriftelijke toestemming van Werkspot."
- **Art. 11.1:** Werkspot mag "zonder dat daartoe een ingebrekestelling vereist is de Overeenkomst … ontbinden en de Vakman uit[sluiten] … zonder verplicht te zijn om eventuele reeds geïnde vergoedingen terug te betalen, indien daar gegronde redenen voor bestaan". Dat geldt onder meer bij (a) "op enige wijze in strijd handelt met deze Algemene Voorwaarden" en (h) een poging de leadprijs te omzeilen.
- **Art. 11.2:** het besluit tot beëindiging wordt "ten minste 30 dagen voordat de beëindiging ingaat" meegedeeld, met reden en feiten. Uitzonderingen staan in art. 11.3 (wettelijke plicht, dwingende reden, herhaalde schending).
- **Art. 16:** interne klachtenprocedure (via support.werkspot.nl/s/contactsupport) en bemiddeling via CEDR voor vakmensen die aan consumenten leveren (16.5).
- **Huisregels:** "Bij klachten doen we onderzoek en op basis van verleden van het vakbedrijf zullen we mogelijk overgaan tot een laatste waarschuwing of verwijdering van het platform."

**6e. Restitutie:** zie §2 (art. 19.2–19.4, letterlijk geciteerd). Aanvullend: art. 17.5 en 18.4 bepalen dat beëindiging de vakman "niet [ontslaat] van de verplichting om de reeds verschuldigde bedragen te voldoen".

**6f. Aansprakelijkheid**
- **Art. 4.1:** "Werkspot heeft daarbij slechts een faciliterende rol en kan dan ook niet verantwoordelijk worden gehouden voor handelen of nalaten van een Gebruiker … Werkspot verleent niet de onderliggende werkzaamheden en treedt niet op als agent voor de Klant of de Vakman."
- **Art. 4.4:** Werkspot garandeert onder meer niet "dat de informatie op het Platform juist, volledig, geschikt, actueel en niet onrechtmatig is, waaronder mede verstaan de door Gebruikers opgegeven informatie". **[interpretatie]** Daaronder vallen dus ook de klusomschrijving en de contactgegevens van de consument.
- **Art. 13.1:** "Werkspot is alleen aansprakelijk voor directe schade die de Vakman lijdt."
- **Art. 13.2:** "De totale aansprakelijkheid van Werkspot bedraagt nooit meer dan de totale vergoeding die Vakman aan Werkspot voor de dienst betaald heeft in de twaalf maanden voordat de schadeveroorzakende gebeurtenis zich voordeed, met een maximum van 500 (vijfhonderd) euro."
- **Art. 13.3:** "Iedere aansprakelijkheid van Werkspot voor indirecte schade, waaronder begrepen maar niet beperkt tot gevolgschade, winstderving en omzetderving, is uitgesloten."
- **Art. 13.4:** "Niets in deze Overeenkomst beperkt de aansprakelijkheid van Werkspot die ontstaan is door opzet of grove schuld aan de zijde van Werkspot of haar senior management."
- **Art. 5.1:** Werkspot mag het platform tijdelijk buiten gebruik stellen "zonder dat hierdoor enig recht op schadevergoeding jegens Werkspot ontstaat".
- **Opdrachtgevers art. 12.3** (alleen voor niet-consumenten, zie 12.1): "De totale aansprakelijkheid van Werkspot zal nimmer meer bedragen dan een bedrag van € 500,00."

**6g. Wijziging van de voorwaarden**
- **Art. 2.2:** wijzigingen worden "ten minste 30 dagen voordat de wijzigingen in werking treden op een duurzame gegevensdrager" gecommuniceerd; de vakman kan tot dat moment opzeggen.
- **Art. 6.7:** voor wezenlijke wijzigingen in de rangschikkingsparameters geldt "doorgaans ten minste vijftien (15) dagen" vooraf.

### Bronnen

| URL | Datum |
|---|---|
| https://www.werkspot.nl/algemene-voorwaarden (vakmensen + opdrachtgevers, versie "maart 2026") | opgehaald 10-11-2026 |
| https://web.archive.org/web/20250811175224id_/https://www.werkspot.nl/algemene-voorwaarden (versie "December 2024") | snapshot 11-08-2025, opgehaald 10-11-2026 |
| https://www.werkspot.nl/blog/faq-brandende-vragen-over-werkspot (€3–€75) | "Bijgewerkt op 24-08-2026"; opgehaald 10-11-2026 |
| https://www.werkspot.nl/blog/faq (€3–€60) | "Bijgewerkt op 24-08-2026"; opgehaald 10-11-2026 |
| https://www.werkspot.nl/blog/nieuw-bij-werkspot-directe-aanvraag | inhoudsdatum onbekend; opgehaald 10-11-2026 |
| https://www.werkspot.nl/blog/cashback-zomeractie-nu-tijdelijk-240-gratis-tegoed-bij-abonnement | actie juni 2017; opgehaald 10-11-2026 |
| https://www.werkspot.nl/blog/werkspot-heeft-een-frisse-nieuwe-look | inhoudsdatum onbekend; opgehaald 10-11-2026 |
| https://www.werkspot.nl/blog/niet-tevreden-over-het-werk-van-de-vakman | opgehaald 10-11-2026 |
| https://www.werkspot.nl/ (homepage, tellers) | opgehaald 10-11-2026 |
| https://www.werkspot.nl/over-werkspot (→ /over-ons) | opgehaald 10-11-2026 |
| https://www.werkspot.nl/hoe-werkt-het (ook /hoe-werkt-het/opdrachtgever → zelfde pagina) | opgehaald 10-11-2026 |
| https://www.werkspot.nl/vakman/registreren | opgehaald 10-11-2026 |
| https://www.werkspot.nl/voorwaarden-voor-reviews | "Updated: 17 Januari 2025"; opgehaald 10-11-2026 |
| https://www.werkspot.nl/kwaliteitseisen (huisregels) | opgehaald 10-11-2026 |
| https://www.sec.gov/Archives/edgar/data/1800227/000110465925030297/tm254280d9_ex99-1.htm (IAC/Angi-spin-off) | 01-04-2025; opgehaald 10-11-2026 |
| https://www.sec.gov/Archives/edgar/data/1705110/000170511026000011/angi-20251231.htm (Angi 10-K FY2025) | ingediend 20-02-2026; **alleen de eerste ±250 KB van 2,5 MB gelezen** (afkapping door web-fetch) |
| https://www.sec.gov/Archives/edgar/data/0001705110/000170511026000104/q32026earningsrelease.htm (Angi Q3 2026) | 03-11-2026; opgehaald 10-11-2026 |
| https://www.bnnvara.nl/kassa/vraag-beantwoord/winkels-webshops/werkspot (gebruikersbijdrage) | 05-04-2019; opgehaald 10-11-2026 |
| https://www.acm.nl/en/node/24822 (P2B-onderzoek, gerelateerde publicaties) | opgehaald 10-11-2026 |

### Niet opgehaald

- **Restitutiebeleid (gronden en termijnen):** de link uit de FAQ (https://www.werkspot.nl/blog/leads-en-restitutie) geeft een 404. Een WebSearch naar support.werkspot.nl-artikelen leverde geen resultaten op. Het tweede alternatief, https://support.werkspot.nl/s/ (Salesforce-helpcenter, met browser-rendering), gaf een time-out na 60 s. De inhoud van het restitutiebeleid is dus onbekend.
- **Huidige abonnementsprijzen en de prijs van gesponsorde plaatsing:** niet op openbare pagina's gevonden; waarschijnlijk alleen zichtbaar na inloggen **[aanname]**. De "afzonderlijke algemene voorwaarden" voor gesponsorde plaatsing (art. 6.8) zijn niet gevonden.
- **Maximum aantal vakmannen per klus/lead:** nergens door Werkspot vermeld.
- **Gemiddelde reviewscore op het platform:** niet gevonden; de betekenis van "Rob 4.9/5" op de homepage is onduidelijk.
- **Nederlandse pers 2024–2026** (Emerce, Sprout/MT, FD, Tweakers, NOS, Kassa-uitzending, Radar): geen Werkspot-specifiek artikel gevonden via WebSearch. Sites zijn niet afzonderlijk doorzocht (credit-zuinigheid).
- **Angi 10-K FY2025:** alleen het eerste deel gelezen. Eventuele toelichtingen verderop over International (bv. minderheidsbelangen, impairments per segment) zijn niet gelezen. Het Q3 2026-10-Q is niet opgehaald.
- **Instapro Group-site** (careers.instapro.group) en MyBuilder/MyHammer-sites: niet opgehaald.
- **Volledige vergelijking van de AV december 2024 met maart 2026:** alleen op trefwoorden vergeleken, niet artikel voor artikel.
<!-- /DEEL1 -->

<!-- DEEL2 -->
## Deel 2 – Reviews en klachten

> Basis: `data/werkspot.csv` na aanvulling (432 rijen; was 129). Nieuwe kolom `reviewer_kant` (vakman / consument / onbekend). Alle tellingen hieronder komen uit een script over de CSV (scratchpad `werkspot/d2/count.py`, uitvoer `werkspot/d2/counts.txt`), opgehaald en gecodeerd op 10-11-2026. Periode nieuwe rijen: 1-11-2024 t/m 10-11-2026. Een review kan meerdere thema's hebben, dus de themakolommen tellen niet op tot n.

### 2.1 Databasis per kant en bron

| bron | vakman | consument | onbekend | hoe opgehaald / gefilterd |
|---|---|---|---|---|
| Trustpilot NL (www.werkspot.nl) | 118 | 206 | 5 | (a) **alle 262** NL-reviews met 1–3★ sinds 1-11-2024 (dataset `l2ugmQlki2nUd1dAo`; nu volledig gelezen, eerder alleen de nieuwste 130); (b) de **nieuwste 70** met 4★ (12-11-2025 t/m 29-10-2026, run `gCil5UCVueyO3WvZz`); (c) de **nieuwste 30** met 5★ (7-10 t/m 10-11-2026, run `T0Xj270LMJZPOD9Bo`). Inhoudsloze reviews ("Dikke NUL sterren", "Alles goed geregeld") en reviews die niet over Werkspot of een via Werkspot ingehuurde vakman gaan, zijn niet opgenomen. |
| Trustpilot EN | 12 | 19 | 0 | alle 44 Engelstalige reviews sinds 1-11-2024 (dataset `abLKBneRXwog0uSxW`, alle sterren) |
| Google Play – Werkspot voor Vakmensen | 32 | – | – | uit deel 1 (200 nieuwste opgehaald; na nr. 100 alles van vóór sept 2023) |
| App Store – Werkspot voor vakmensen | 23 | – | – | uit deel 1 |
| App Store – Werkspot (consumenten-app, id1568256243) | 3 | 5 | 6 | **nieuw**: alle 52 reviews opgehaald (run `5fPEcR8zqNGGgUaSs`), 14 vanaf nov 2024 opgenomen. De app wordt door beide kanten gebruikt. |
| Radar-forum (AVROTROS) | 3 | – | – | uit deel 1, oud (2018–2019) |
| **totaal** | **191** (172 sinds nov 2024) | **230** (alle sinds nov 2024) | **11** | |

**Groepen** (1 ster / midden = 2–3★ plus 4–5★ mét concreet klachtpunt / positief = 4–5★ zonder klacht):

| kant | 1 ster | midden | positief | geen score |
|---|---|---|---|---|
| vakman | 158 | 28 | 2 | 3 |
| consument | 86 | 66 | 78 | – |
| onbekend | 6 | 5 | 0 | – |

Niet gevonden of niet op te halen (gezocht via WebSearch op 10-11-2026): Kassa/Radar/Consumentenbond/FD en Tweakers leverden **geen** artikel uit 2025–2026 over Werkspot-leadkosten of consumentenklachten op. Alleen de oude Radar-forumdraden en Werkspot's eigen pagina's kwamen terug. Reddit is voor de zoektool geblokkeerd (domein niet toegankelijk). Een Google Play-versie van de consumenten-app is niet gevonden. LinkedIn, Facebook-groepen en YouTube zijn niet doorzocht om credits te sparen. Er staan dus **geen citaten uit nieuwsmedia of fora van ná 2019** in deze analyse.

### 2.2 Codeboek-uitbreiding en mapping

Nieuwe vakman-codes. De oude codes blijven staan, de fijnere codes komen erbij:

| oude code | fijnere code(s) | regel |
|---|---|---|
| `leadkosten` (het model: betalen per contact) | `leadprijs` | klacht over de hoogte of willekeur van het bedrag per lead (€-bedragen, "te hoog", "duur") |
| `leadkwaliteit` | `klant-reageert-niet`, `fout-nummer`, `prijs-shoppers`, `buiten-werkgebied` | klant reageert niet of verdwijnt; nummer/e-mail klopt niet; klant wil alleen een prijsindicatie of de goedkoopste; lead buiten de regio |
| `support` | `restitutie` | geld-terugverzoek afgewezen, traag of verrekend |
| `lock-in` | `abonnement-contract`, `account-geblokkeerd`, `reviews-kwijt` | abonnement of contract niet op te zeggen; account geblokkeerd; opgebouwde reviews kwijt |
| `bugs`/`mobiel` | `app` | elke klacht over de app of website |
| – | `lead-concurrentie` (bestond al), `zichtbaarheid-ranking` | lead aan veel vakmannen verkocht; minder aanvragen na een slechte review |
| – | `transparantie-consument` | **extra code**: vakman vindt dat de consument niet weet dat contact delen de vakman geld kost |

Consument-codes: `te-veel-reacties`, `te-weinig-reacties`, `kwaliteit-vakman`, `gespamd-gebeld` (ook: te veel mails en reviewverzoeken, ongevraagd gebeld), `nepreviews`, `prijsonzekerheid` (rekening hoger dan afgesproken of geen prijsindicatie), `no-show`, `geen-garantie`, `privacy`, `positief:<onderwerp>`. Extra codes, omdat de tekst daar duidelijk om vroeg:
- `fraude`: aanbetaling of voorschot weg, oplichting.
- `screening`: Werkspot controleert vakmannen (KvK, bevoegdheid) niet.
- `geschil-geen-steun`: Werkspot bemiddelt niet en verwijst door naar het Juridisch Loket of de politie.
- `review-systeem`: review kan niet geplaatst worden, wordt verwijderd, of er komt een reviewverzoek voor het verkeerde bedrijf.
- `leadmodel-voelbaar`: de consument merkt het leadmodel (dringerige of geïrriteerde vakman, "reageren kost ons geld").
- `matching-regio`: vakmannen niet uit de buurt.

**Hoe gecodeerd**: nieuwe rijen (303) zijn handmatig gecodeerd. Bij de 118 bestaande vakmanrijen zijn de fijnere codes **op trefwoord** toegevoegd (regels in `werkspot/d2/build.py`; een steekproef van 8 rijen is nagelopen en één fout patroon is gecorrigeerd: "telefonisch niet bereikbaar" ging over Werkspot, niet over de klant). Bij die oude rijen zijn de fijnere codes dus een **ondergrens**: `restitutie` staat bijvoorbeeld bij 10 oude rijen, terwijl `support` daar vaak ook afgewezen restitutie betekent. De 11 bestaande consumentrijen zijn handmatig bijgecodeerd. Bij 14 dubbele URL's zijn de thema's samengevoegd.

### 2.3 Vakmannen (n = 191; 172 sinds nov 2024)

**Thema's** (top, met verdeling over de groepen):

| # | thema | totaal | 1★ | midden | positief |
|---|---|---|---|---|---|
| 1 | `leadkosten` (betalen per contact, vóór er werk is) | 159 | 136 | 21 | 0 |
| 2 | `leadprijs` (hoogte/willekeur, €3–€120 genoemd) | 92 | 73 | 17 | 0 |
| 3 | `leadkwaliteit` | 81 | 72 | 9 | 0 |
| 4 | `support` (geen telefoon, standaardmails, incasso) | 67 | 62 | 4 | 0 |
| 5 | `klant-reageert-niet` | 47 | 44 | 3 | 0 |
| 6 | `lead-concurrentie` (5–10+ vakmannen per klus) | 39 | 33 | 6 | 0 |
| 7 | `restitutie` | 28 | 27 | 1 | 0 |
| 8 | `app` | 18 | 12 | 6 | 0 |
| 9 | `prijs-shoppers` | 16 | 15 | 1 | 0 |
| 9 | `transparantie-consument` | 16 | 14 | 1 | 0 |
| 11 | `lock-in` 10 · `fout-nummer` 9 · `account-geblokkeerd` 8 · `onboarding` 7 · `ontbrekend:review-bezwaar` 6 · `abonnement-contract` 5 · `ontbrekend:dubbele-opt-in` 4 · `ontbrekend:betalen-per-opdracht` 3 · `buiten-werkgebied` 1 · `zichtbaarheid-ranking` 1 · `reviews-kwijt` 1 (ondergrens, zie 2.2) | | | | |

**1 ster (158).** Dit is het bekende beeld uit deel 1, nu met twee keer zoveel data. Er komen drie dingen bij:
- *Lead-concurrentie gekoppeld aan een rekensom*: "meer dan 200 klanten aangeschreven. Resultaat? Slechts 4 opdrachten en … bijna €1000 kwijt aan leadkosten" (Trustpilot NL, 2025-08-07).
- *Het filter is weggehaald*: "Vroeger kon je ook nog filteren op aantal reacties als professional. Dit hebben ze er nu bewust uitgehaald" (Trustpilot NL, 2025-08-29).
- *Klant kan zonder gesprek accepteren*: "zonder enige chat/gesprek worden gegevens doorgestuurd en geld in rekening gebracht" (Trustpilot NL, 2025-03-13).

**Midden (28) – waar de nuance zit.** Middenreviewers wijzen het model niet af. Hun bezwaar is de verhouding en het moment van betalen:
- `leadprijs` niet in verhouding tot de klusgrootte (17 van 28): "Op zich geen slecht model, was het niet dat de kosten erg uit verhouding zijn met de opbrengsten. Een lead/opdracht die 2 uur kost … soms wel €20." (Trustpilot NL, 2026-02-07, 2★); "Voor een koffietafel enkel een nieuwe laklaag is er een commisie van 37 euro" (App Store, 2024-11-01, 2★).
- Betalen bij contact in plaats van bij opdracht: "dat de leadprijs bij contact wordt verrekend in plaats van inhuur" (Google Play, 2026-03-01, 2★).
- Volume is er wel, conversie niet: "Ik krijg redelijk veel klanten, ben ik super blij mee. Maar 2 op 5 … alleen een berichtje van we hebben al iemand gevonden … wel een leadprijs" (Trustpilot NL, 2025-05-25, 2★).
- `app` (6 van 28): "app moet 3 of 4 keer per maand opnieuw geïnstalleerd worden" (Google Play, 2026-04-19, 2★).
- Transparantie: "De opdrachtgevers zijn niet op de hoogte dat de vakman een prijs betaald … Dit schrikt vakmensen af en laat opdrachtgevers met een opdracht zitten waar niet op wordt gereageerd." (Trustpilot NL, 2026-08-05, 2★)

**Positief (2) + gemengd.** Echt positieve vakmanreviews zijn zeldzaam: "Door Werkspot heb ik regelmatig Werk en ben dik tevreden" (Trustpilot NL, 2026-11-05, 5★); "Good company, plenty of jobs found here" (Trustpilot EN, 2024-11-27, 5★). Twee 5★-reviews uit deel 1 noemen zelf een klacht over de leadprijs en staan daarom nu in "midden".

### 2.4 Consumenten (n = 230; allemaal sinds nov 2024)

**Thema's:**

| # | thema | totaal | 1★ | midden | positief |
|---|---|---|---|---|---|
| 1 | `kwaliteit-vakman` (prutswerk, taal, schade) | 48 | 35 | 13 | 0 |
| 2 | `fraude` (aanbetaling weg, oplichting) | 32 | 27 | 5 | 0 |
| 3 | `screening` (KvK/bevoegdheid niet gecontroleerd) | 29 | 12 | **17** | 0 |
| 4 | `prijsonzekerheid` | 21 | 14 | 7 | 0 |
| 4 | `no-show` | 21 | 16 | 5 | 0 |
| 6 | `geschil-geen-steun` | 20 | 16 | 4 | 0 |
| 7 | `gespamd-gebeld` | 16 | 8 | 8 | 0 |
| 7 | `te-weinig-reacties` | 16 | 2 | **14** | 0 |
| 9 | `geen-garantie` | 14 | 12 | 2 | 0 |
| 10 | `review-systeem` 13 · `privacy` 9 · `nepreviews` 8 · `leadmodel-voelbaar` 8 · `gebruiksgemak` 8 · `bugs` 6 · `support` 6 · `te-veel-reacties` 3 · `matching-regio` 3 | | | | |
| + | `positief:vakman` 52 · `positief:snelheid` 37 · `positief:gemak` 20 · `positief:keuze` 11 · `positief:matching` 10 · `positief:reviews` 6 · `positief:betrouwbaar` 4 · `positief:concept` 4 | | | | |

**1 ster (86).** Hier gaat het vooral over de **vakman**, niet over Werkspot: prutswerk, een aanbetaling die verdwijnt, of iemand die niet komt opdagen. Werkspot krijgt de rekening omdat het niet screent en niet bemiddelt:
- "Werkspot doet niets en verwijst mij door naar het Juridisch loket. … Ben overgestapt naar Klusup, geeft meer vertrouwen omdat alle betalingen via Klusup gaan." (Trustpilot NL, 2025-12-03)
- "Een bedrijf dat zich voor het eerst aanmeldt bij Werkspot mag zelf voor de eerste 5 reviews zorgen … Dit betekent dus dat deze heel goed nep kunnen zijn!" (Trustpilot NL, 2025-03-15)
- Privacy: "Angry trader called me without me providing my phone number, he told me he got it from werkspot for 30 euros." (Trustpilot EN, 2025-03-17)

**Midden (66) – de meeste aandacht.** Drie patronen vallen op:
1. **Te weinig reacties** (14 van 66). Dit is het spiegelbeeld van de vakmanklacht over leadprijs en concurrentie: "Van de 10 bedrijven die ik selecteren kon hebben er maar 3 gereageerd … Probleem is waarschijnlijk dat bedrijven die reageren sowieso … een bedrag moeten betalen" (Trustpilot NL, 2026-10-02, 3★); "Van de 5 uitgenodigde bedrijven heeft slechts 1 gereageerd, maar hiermee heeft mijn zoektocht uiteindelijk een prima match opgeleverd." (Trustpilot NL, 2026-04-20, 4★). Een vakman bevestigt het mechanisme: "Dit komt omdat steeds meer klanten 'alleen maar een prijsje' willen weten. De vakman moet echter betalen … dus wordt hij heel selectief!" (Trustpilot NL, 2025-02-08, 1★).
2. **Screening / betrouwbaarheid** (17 van 66): tevreden over het platform, wantrouwig over het aanbod. "het werkt en het idee is geweldig … maar: er zitten een enorme hoeveelheid charlatans op" (Trustpilot NL, 2026-06-05, 3★); "Nagenoeg alle reacties bleken helemaal niet de bevoegdheid te hebben om het werk uit te voeren." (Trustpilot NL, 2026-07-13, 3★).
3. **Ruis en kleine ergernissen** (`gespamd-gebeld` 8, `gebruiksgemak` 7): te veel reviewverzoeken vóór de klus, reacties slecht te vergelijken, chat-inbox zonder ongelezen-markering. "het na enkele dagen al spammen met de vraag om een review terwijl de klus pas maanden later zou plaatsvinden" (Trustpilot NL, 2026-10-16, 4★); "De reacties op de klus zijn niet eenvoudig te beoordelen en te vergelijken." (Trustpilot NL, 2026-07-09, 4★).

Ook in het midden: consumenten merken het leadmodel zelf: "Als klant wil je offertes kunnen vergelijken zonder dat je je schuldig hoeft te voelen. … Ik zou liever abonnementskosten … zien" (Trustpilot NL, 2024-12-30, 1★); "Helaas kost het de dienstverlener al geld om überhaupt in contact te komen. … Kan beter met een achteraf systeem" (Trustpilot NL, 2026-09-21, 4★).

**Positief (78).** Kort en algemeen. 36 van de 78 gaan vooral over de **vakman** (netjes gewerkt, afval meegenomen), niet over het platform. Over het platform: snelheid (27), gemak (14), keuze (10). "Ervaring met Werkspot: ruime keuze, snel een aanbod." (Trustpilot NL, 2026-08-24, 4★); "Na een selectie kan ik met gerust hart obv reviews, de klus uit handen geven." (Trustpilot NL, 2026-10-07, 5★).

### 2.5 Wat beide kanten expliciet waarderen

| waardering | vakman | consument |
|---|---|---|
| **Volume / snel contact**: veel aanvragen of snel reacties | `positief:aanbod` 4 ("Ik krijg redelijk veel klanten", 2025-05-25) | `positief:snelheid` 37, `positief:keuze` 11 |
| **Het concept** (vraag en aanbod bij elkaar, geen eigen marketing nodig) | `positief:concept` 2 ("Op zich een mooi platform voor mensen die niet zo goed zijn in netwerken", 2025-03-04) | `positief:concept` 4; "Ook fijn dat je niet afhankelijk bent van de SEO skills van vakmensen" (2024-12-30) |
| **Reviews als vertrouwensanker** | reviews zijn waardevol, en juist daarom doet verlies pijn (`account-geblokkeerd` 8) | `positief:reviews` 6, maar tegelijk `nepreviews` 8 en `review-systeem` 13 |
| **Werkende app/chat** | `positief:app` 4 (meestal mét klacht) | `positief:gemak` 20 |

Beide kanten waarderen dus hetzelfde: **snel een match en een geloofwaardig reviewprofiel**. Over prijs zegt geen van beide kanten iets positiefs. Eén consument noemt "duidelijk prijs" (2026-03-19) en één "vlot een richtprijs" (2026-10-27).

### 2.6 "Wat net mist": concrete wensen

**Vakmannen:**
1. **Betalen bij opdracht of na wederzijdse bevestiging**, niet bij contact: "Werkspot zou dit anders moeten gaan vormgeven … pas de lead te laten betalen door ondernemer nadat de klus gegarandeerd doorgaat" (Trustpilot NL, 2026-05-17); "maak dit systeem anders dat je beide mee eens moet zijn om gegevens te delen" (2025-01-15). Telling: `ontbrekend:dubbele-opt-in` 4 + `ontbrekend:betalen-per-opdracht` 3, en het komt impliciet terug in tientallen `leadkosten`-rijen.
2. **Maximaal 3–4 vakmannen per klus**, of het filter op aantal reacties terug: "Het aantal vakmensen per opdracht beperken" (2026-05-06); "MAXIMAAL 3 TOT 4 MAN" (2026-02-18).
3. **Consument informeren** dat contact delen geld kost (`transparantie-consument` 16): "werkspot moet als koptekst aan consumenten laten weten dat 'chat starten' vakmensen geld kost!!" (2026-07-05).
4. **Leads verifiëren en aanvragen completer maken** (foto's, maten): "strengere eisen stelt aan de volledigheid van aanvragen en de contactkosten herziet wanneer een opdrachtgever vrijwel direct afhaakt" (2026-09-05); "Bellen klanten nooit na om te bevestigen of het wel 'echt' een lead is" (2026-07-05).
5. **Leadprijs die past bij de klusgrootte** en niet zonder aankondiging wijzigt (2026-08-07 verwijst naar art. 19.7 AV).
6. **Hoor en wederhoor bij slechte reviews** in plaats van direct blokkeren; reviews splitsen in klant/vakman (2025-08-13).
7. **Bereikbare support** (telefoon) en een opzegknop voor het abonnement (2025-08-27 EN; 2026-05-06).

**Consumenten:**
1. **Screening van vakmannen** (KvK, bevoegdheid, verzekering): "Goed screenen is noodzaak." (2025-04-04, 3★).
2. **Bemiddeling of geldbescherming bij conflicten**: betaling via het platform of escrow ("alle betalingen via Klusup", 2025-12-03).
3. **Betrouwbaardere reviews**: negatieve reviews niet weghalen, geen zelf-aangeleverde eerste 5 reviews, en een besloten enquête per vakman (netjes, veilig, spreekt Nederlands, komt afspraken na) (2026-06-05).
4. **Meer en serieuzere reacties**, en niet-reagerende bedrijven kunnen melden of laten verwijderen (2026-04-28, 4★).
5. **Minder mails**: reviewverzoek pas na de klus, en een uitschrijfoptie (2026-10-16; 2025-05-11).
6. **Offertes naast elkaar kunnen vergelijken** en de vestigingsplaats zien (2026-07-09; 2026-10-31).
7. **Telefoonnummer pas delen na eigen akkoord** (2026-01-19 EN; 2025-05-25 EN).

### 2.7 Vertekening

- **Filter per bron**: de 1–3★ op Trustpilot NL zijn volledig gelezen (262). Van 4★ en 5★ alleen de nieuwste 70 en 30. De consumentenkant is daardoor representatiever voor de kritische reviews dan voor de positieve.
- **Volumeverhouding** (afgeleid, **[aanname]** bij extrapolatie): Trustpilot meldt 7.675 reviews en een TrustScore van 4 voor www.werkspot.nl (veld `companyTotalReviews`/`companyTrustScore`, opgehaald 10-11-2026). Er zijn 262 NL-reviews met 1–3★ in 24 maanden (~11 per maand). De 30 nieuwste 5★ vallen in ruim één maand en de 70 nieuwste 4★ in bijna twaalf maanden. Ruwe schatting: de NL-reviews van de laatste 24 maanden zijn grotendeels 5★, en ~1 op 4 à 5 is kritisch.
- **Vakman vs consument op Trustpilot NL**: binnen 1–3★ is het ongeveer half om half (117 vakman tegen 118 consument opgenomen; 5 onbekend; ~22 inhoudsloos of niet relevant). Binnen de 100 bekeken 4–5★ staat **1** vakman. Vakmannen zijn op Trustpilot dus vrijwel alleen boos aanwezig. Trustpilot nodigt vooral consumenten uit na een klus. Veel 4–5★ gaan daardoor over de individuele vakman ("Harde werker"), niet over Werkspot.
- **Boze-reviewer-bias**: vakmannen schrijven vooral als ze stoppen of geld kwijt zijn. Er zijn vrijwel geen tevreden vakmanstemmen (2 positief van 191). Hun ontevredenheid is robuust (alle bronnen, zelfde patroon), maar *hoeveel* vakmannen ontevreden zijn, is niet te kwantificeren. Vakmannen moedigen elkaar ook aan om te reviewen ("Lees alle 1 ster reviews vakmensen!", 2026-10-27, niet opgenomen).
- **Kantbepaling**: `reviewer_kant` volgt uit de tekst ("als vakman", "leads", "ik heb een klus geplaatst"). 11 rijen zijn **onbekend** (o.a. korte app-reviews). Consumentenreviews over fraude zijn soms niet te verifiëren en gaan vaak over één bedrijf.
- **Bron-mix**: vakmanrijen komen voor 62% van Trustpilot NL en voor 29% uit de vakman-apps. Consumentrijen komen voor 90% van Trustpilot NL. Geen forum- of nieuwsbron uit de laatste 24 maanden.

### Bronnen (opgehaald 10-11-2026)
- Trustpilot www.werkspot.nl via Apify `automation-lab/trustpilot`: datasets `l2ugmQlki2nUd1dAo` (NL 1–3★ sinds 2024-11), `K6NeBaw03VWwymmIy` (NL 4★), `oo8yLe6tdi2Gvdi8E` (NL 5★), `abLKBneRXwog0uSxW` (EN). Review-URL's staan per rij in de CSV (https://www.trustpilot.com/reviews/<id>).
- App Store "Werkspot" https://apps.apple.com/nl/app/werkspot/id1568256243 via `thewolves/appstore-reviews-scraper`, dataset `1SOXuymGB7tRxeJik`.
- Vakman-apps en Radar-forum: zie deel 1 / `analyse/werkspot.md`.
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
