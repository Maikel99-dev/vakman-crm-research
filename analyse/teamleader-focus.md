# Teamleader Focus – review-analyse

> Teamleader Focus is een **algemeen** CRM/offerte/facturatie-pakket voor kmo's (België/Nederland), geen vakbedrijf-software. Weinig reviewers zijn aantoonbaar bouw-, installatie- of vakbedrijven. Het veld `reviewer_type` geeft aan wanneer dat wel zo is. Inzichten over offerte, facturatie, koppelingen, de mobiele app en prijs zijn wel goed overdraagbaar.

## Profielschets

- **Doelgroep**: kmo's, zelfstandigen en dienstverleners, vooral in België (Gent) en Nederland. Volgens Capterra.nl zit het pakket ook in de categorie "CRM voor de bouw" (opgehaald 10-11-2026).
- **Prijsindicatie**: Capterra.nl noemt een "Beginprijs € 37,50 / maand" met gratis proefversie (opgehaald 10-11-2026). Reviewers op Trustpilot noemen:
  - jaarcontracten met automatische verlenging,
  - "standaard voor twee teamleden" (2024-04-22),
  - een stijging van "650 euro en nu ruim 1100 per jaar voor EEN GEBRUIKER" (2024-07-03).
- **Kernfuncties**: CRM (contacten, deals/pipeline), offertes met digitale ondertekening en "bekeken"-tracking, facturatie met boekhoudkoppelingen (o.a. Yuki) en Peppol, projecten, urenregistratie, agenda/planning, werkbonnen, tickets en een API/marketplace. Er is een mobiele app: Android `eu.teamleader.focus`, iOS id6453793095. De nieuwe app (v3) kwam in augustus/september 2023.

## Databasis

| Bron | In CSV | 1★ | 2★ | 3★ | 4★ | 5★ | Opmerking |
|---|---|---|---|---|---|---|---|
| Google Play (NL; BE gaf dezelfde 16 reviews) | 15 | 5 | 2 | 3 | 1 | 4 | Alle reviews met inhoud. 1 review zonder inhoud (alleen een naam) weggelaten |
| App Store NL | 7 | 1 | – | 5 | – | 1 | Alle |
| App Store BE (nl) | 6 | 2 | 1 | 1 | 1 | 1 | Alle |
| Trustpilot NL-talig (`teamleader.eu`) | 39 | 15 | 3 | 1 | 3 | 17 | Selectie uit de 100 nieuwste NL-reviews (scraper, max. 100). **Alle** 1–3★ en kritische 4★ zijn opgenomen. Van de positieve alleen die met inhoud over offerte, facturatie, koppelingen, onboarding en gebruiksgemak. Ca. 60 korte lofreviews ("top service") zijn niet opgenomen |
| Trustpilot EN | 2 | – | 1 | – | 1 | – | Uit de 8 reviews in de Engelse standaardweergave |
| Capterra.nl | 5 | 1 | 1 | – | 2 | 1 | Van de 45 reviews (gemiddeld 4,2). Pagina 1 en de "meest relevante" selectie: bouwmaterialen, installatiebouw en kritische reviews |
| **Totaal** | **74** | | | | | | |

- **Verdeling (script)**: 1 ster: 24 · midden: 25 · positief: 25. Dit is **geen** representatieve verdeling, want kritische reviews zijn bewust oververtegenwoordigd. Trustpilot heeft in totaal 275 reviews en een TrustScore van 4,1. Capterra.nl geeft 4,2 en meldt 84% positief sentiment.
- **Periode**: 2020-09 – 2026-10. Sinds nov. 2024: 27 rijen (11× 1★, 5× midden, 11× positief). De meeste app-reviews zijn van 2023–2025. De Capterra-reviews zijn ouder (2020–2024) en apart gemarkeerd.
- **Reviewer-type**: aantoonbaar bouw, installatie of vakwerk: 4 rijen.
  - Trustpilot 2026-08-10, "vakmensen, plaatsers… maatwerk"
  - Trustpilot 2023-04-13, overstap naar Bouwsoft
  - Capterra, bouwmaterialen
  - Capterra, machine- en installatiebouw

  Daarnaast een AV-integrator en meerdere app-reviewers met buitendienst of werkbonnen. De rest zijn algemene kmo's.
- **Kwaliteitsnoot**:
  - Trustpilot bevat veel korte 5-sterrenreviews over support die de naam van een medewerker noemen ("Thijs", "Nathan", "Floor"). Dat wijst op uitnodigingen na supportcontact. Positieve Trustpilot-scores zijn daardoor minder informatief.
  - De Trustpilot-scraper gaf zonder taalfilter maar 8 (Engelse) reviews. Met het filter `nl` kwamen er 100.
  - G2 is niet opgehaald: g2.com is DNS-geblokkeerd voor WebFetch, en gerenderd ophalen via Apify gaf bij eerdere tools een time-out. Omdat Capterra.nl en Trustpilot al ruim voldoende data gaven, heb ik dat niet opnieuw geprobeerd.
  - Capterra.com en OMR zijn niet opgehaald (zuinig met credits).
  - De Capterra-filter op sector (bouw/installatie) werkte niet via een URL-parameter.

## Wat gebruikers goed vinden (de lat)

- **Offerte, akkoord en factuur in één flow, met inzicht wanneer de klant de offerte opent**: "kan ik precies zien hoe vaak mijn klanten de offerte hebben bekeken, wat me helpt om op het juiste moment te volgen… factuur automatisch koppelen aan mijn boekhoudprogramma Yuki" (Trustpilot, 2024-07-26). En: "Klanten kunnen met 1 klik hun samenwerking bevestigen." (Trustpilot, 2025-03-05).
- **Eén dossier dat het hele team kan inzien**: "Van offerte tot factuur, de hele flow zit gecentraliseerd zodat iedereen in het team op elk moment kan zien hoever een bepaald dossier staat." (Trustpilot, 2024-08-13).
- **Koppelingen en API**: "eenvoudige integraties met o.a. mijn boekhoudpakket en Zapier" (Trustpilot, 2025-09-30). "HEEL veel mogelijkheden met een strakke API" (Trustpilot, 2025-05-02). Ook Peppol-facturatie wordt gewaardeerd (Trustpilot, 2025-05-26).
- **Gebruiksgemak**: "De grote kracht van Teamleader is het gebruiksgemak. Alles is duidelijk, logisch opgebouwd" (Trustpilot, 2026-09-21).
- **Flexibele workflow per projecttype**, van een AV-integrator: "Teamleader volgt voor elk type onze manier van werken" (Trustpilot, 2025-09-29).
- **Leverbon op locatie laten tekenen en direct factureren**: "De klant tekent de leverbon en de factuur zit met een simpele druk op de knop zo in de bus." (Trustpilot, 2022-08-03, oud).

## Top 5 pijnpunten

Frequentie is het aantal CSV-rijen met dat thema (telscript `count2.py`), uitgesplitst naar 1★ / midden / positief. Let op de selectiebias die hierboven is beschreven.

| # | Thema | Frequentie (1★/midden/pos.) | Ernst |
|---|---|---|---|
| 1 | **mobiel**: app-stabiliteit, uitloggen, ontbrekende functies | 29 (9/14/6) | Hoog: monteur of buitendienst kan niet werken ("werkbonnen zo niet maken") |
| 2 | **bugs** / stabiliteit (vooral de app; ook uren die niet op de factuur kloppen) | 19 (10/9/0) | Hoog |
| 3 | **prijs**: duur, minimum 2 gebruikers, prijsverhogingen | 18 (10/7/1) | Hoog voor kleine bedrijven |
| 4 | **lock-in**: jaarcontract, stilzwijgende verlenging, deurwaarder, lastige data-export | 13 (11/2/0) | Hoog: het meest emotionele thema bij 1★ |
| 5 | **support**: alleen mail of ticket, traag, verwijzing naar algemene voorwaarden | 14 (8/5/1). Ook 9× `positief:support` | Middel: support is gepolariseerd |

Daarna volgen gebruiksgemak/inflexibiliteit (9), planning in de app (8), onboarding (7), werkbon (5) en offerte-opvolging in de app (5).

**1. De mobiele app**
- "De app loopt telkens vast na het inloggen! Ik kan mijn werkbonnen zo niet maken dit is een administratie ramp!" (Google Play, 2024-11-27)
- "Helaas praktisch onbruikbaar. Incompleet, instabiel, buggy en niet native" (App Store NL, 2025-02-03)
- "zodra de internetverbinding even wegvalt, je meteen wordt afgemeld" (Google Play 4★, 2024-07-31)

**2. Bugs en data die niet klopt**
- "Op onverklaarbare wijze worden uren op facturen geplaatst en komen tijdsregistraties niet met de factuur overeen." (Trustpilot, 2024-06-03)
- "werkbon niet automatisch aan project gekoppeld… bon niet factureerbaar" (App Store BE, 2024-03-21)
- "er nog steeds dagen weg vallen wanneer je in de agenda scrollt" (App Store NL, 2025-01-10)

**3. Prijs en prijsmodel**
- "Het grootste nadeel vind ik de prijs; die is erg hoog en standaard voor twee teamleden." (Trustpilot 4★, 2024-04-22)
- "Het was 650 euro en nu ruim 1100 per jaar voor EEN GEBRUIKER." (Trustpilot, 2024-07-03)

**4. Lock-in, contract en export**
- "opzie tegen de mutatie van alle gegevens naar een vergelijkbaar systeem van een concurrent. Dat is echt de enige reden dat ik nog niet ben weggegaan." (Trustpilot, 2026-10-21)
- "14 dagen voor automatische verlenging hebben we het abonnement opgezegd, om nu te horen dat dat 1 dag te laat is" (Trustpilot, 2024-01-18)
- "Als je weg gaat krijg je je gegevens niet in een eenvoudig om te zetten format." (Capterra.nl, 2020-09-08, oud)

**5. Support**
- "alleen bereikbaar via mail en \"binnen\" 24 uur antwoord ... op BELGISCHE werkdagen" (Trustpilot, 2024-06-03)
- "Ze komen ter plaatse alles uitleggen tot je klant bent… is 12 km te ver en moet het via Teams." (Trustpilot, 2026-10-07)

**Signaal uit de vakbranche (1 review, maar zeer relevant)**
- "Zodra je maatwerk doet, zelf plaatst of projecten hebt die variëren per klant, wordt het een ramp. Niets wordt automatisch berekend… Je werkt letterlijk drie keer aan hetzelfde project om één offerte klaar te krijgen… Voor vakmensen, plaatsers of bedrijven die maatwerk doen, is dit programma geen hulp maar een last." (Trustpilot, 2026-08-10)

## "Wat net mist" (middenreviews)

1. **De app moet even goed zijn als het platform, vooral voor de buitendienst.** "De app reflecteert niet de rest van het platform." (App Store BE 2★, 2023-10-06). Concreet ontbreekt:
   - direct bellen vanuit een geplande call, en het gesprek automatisch registreren (Google Play 3★, 2023-08-22; App Store BE 2★)
   - pushmeldingen voor calls, taken en afspraken (App Store BE 2★)
   - "een gespreksverslag… met vervolgactie. Dit is essentieel voor buitendienst" (App Store NL 3★, 2023-09-15)
   - een collega toevoegen aan een afspraak (App Store NL 5★ met minpunten, 2023-12-30)
2. **WhatsApp vanuit het klantdossier.** "Met de oude app kon ik nog linkjes naar whatsapp openen… Sinds de nieuwe app kan dat niet" (Google Play 2★, 2024-05-14). Teamleader antwoordde dat de koppeling met WhatsApp "op onze planning [staat] om te bekijken".
3. **Offline blijven werken en ingelogd blijven.** Uitloggen bij slecht bereik of na updates komt in 6 app-reviews terug (inlog- of uitlogproblemen).
4. **Hulp bij de inrichting na de verkoop.** "iets meer meedenken over hoe Teamleader het beste in te richten voor ons en hoe de budgetten te monitoren" (Trustpilot 3★, 2026-03-30). En: "het vereist wel een investering van zowel tijd als geld" (Trustpilot 4★, 2024-09-17).
5. **Een prijsmodel voor één gebruiker.** "Ik werk alleen en zou liever een uitgekleed pakket hebben voor mijzelf" (Trustpilot 4★, 2024-04-22).

## Kansen voor ons CRM

- **Offerte-opvolging naar Teamleader-niveau tillen, met calculatie voor maatwerk.** Gebruikers waarderen "offerte bekeken"-tracking, tekenen met 1 klik en omzetten naar factuur. Dat is de minimumeis. Waar Teamleader faalt voor vakmensen, is calculatie voor maatwerk en plaatsing (materiaal plus arbeid per klus). Een offertemodule met calculatie per klus, gekoppeld aan automatische herinneringen als de klant de offerte geopend maar niet getekend heeft, is een directe kans.
- **WhatsApp in het klantdossier.** Er is een expliciete vraag in de middenreviews en Teamleader heeft het nog niet. Denk aan: een gesprek starten en terugzien per klant of adres, en aanvragen via WhatsApp opvangen.
- **Een monteur-app die nooit uitlogt en offline werkt**, met werkbon, foto's en handtekening, en een werkbon die automatisch aan project en factuur gekoppeld is. Dit is het grootste pijnpunt bij Teamleader en voor vakbedrijven essentieel.
- **Gespreksverslag met vervolgactie na een bezoek of opname** (buitendienst), plus pushmeldingen. Dit sluit aan op offerte-opvolging na een opname op locatie.
- **Eerlijke contractvoorwaarden als verkoopargument**: maandelijks opzegbaar, volledige data-export (inclusief notities), geen minimum van 2 gebruikers. Lock-in en prijsverhogingen zijn de bron van de meeste 1-sterrenreviews.
- **Hulp bij de inrichting door mensen uit de branche** (standaardworkflows voor dakdekker, installateur of schilder). Dat beantwoordt de "meedenken bij inrichting"-klacht en voorkomt dure implementaties.
- **Klantdossier per adres en nazorg/onderhoud**: Teamleader-reviewers noemen het centrale dossier als kracht, maar niemand noemt adres- of objectgebaseerd werken of onderhoudscontracten. Dat dit ontbreekt is dus niet onderbouwd door reviews. Het blijft een hypothese die past bij de "maatwerk/plaatsers"-klacht.
