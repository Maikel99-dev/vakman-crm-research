# Werkspot (leadplatform) – wat vakmannen zeggen

> Leadplatform, dus andere bril dan bij CRM-tools: dit gaat over **vakmannen die leads kopen**, niet over consumenten.
> Extra codes voor deze tool (bovenop het codeboek in README): `lead-concurrentie` = aan hoeveel vakmannen dezelfde lead wordt verkocht / prijsstrijd per lead; `ontbrekend:review-bezwaar` = geen hoor-en-wederhoor bij negatieve reviews; `ontbrekend:dubbele-opt-in` = vakman wil pas betalen na wederzijdse bevestiging.

## Profielschets

- **Wat**: grootste NL-klussenplatform, onderdeel van Instapro (MyBuilder UK, Travaux.com, etc.; eerder Angi). Consument plaatst gratis een klus, vakmensen reageren ("interesse"), consument deelt contactgegevens → op dat moment betaalt de vakman de lead.
- **Doelgroep vakkant**: zzp'ers en kleine bedrijven in klussen/bouw/installatie/schilderwerk/tuin. Uit de reviews: veel zzp'ers en starters, ook installateurs, badkamerspecialisten, schilders, beveiligingsinstallateur, timmerman.
- **Prijsmodel** (bron: werkspot.nl/blog/faq-brandende-vragen-over-werkspot, CMS-datum 24-08-2026 – die datum staat op alle blogs en zegt niets over wanneer deze prijs is ingegaan; een tweede FAQ-pagina noemt €3–60; opgehaald 10-11-2026; zie `werkspot-diepte.md` deel 1): "De leadprijs … kan variëren van € 3,00 tot € 75,00", bepaald op basis van wat de consument invult (vakgebied, oppervlakte, hoeveelheid, materiaal). Lead = naam, e-mail, telefoon. Kosten worden in rekening gebracht "wanneer een consument bij wederzijdse interesse contactgegevens met jou deelt"; maandelijkse facturatie. Werkspot: "Het platform is zo ontworpen dat de inkomsten uit de opdrachten … na verloop van tijd al jouw leadkosten dekken." Daarnaast melden enkele vakmannen een maandabonnement (bv. "ongeveer 70 euro" per maand) – de abonnementsvoorwaarden zelf zijn niet opgehaald.
- **Kernfuncties vakkant**: app "Werkspot voor Vakmensen" (Android `com.werkspot`, iOS id1319263901), opdrachtenfeed op vakgebied/werkgebied, chat met opdrachtgever, directe aanvragen, profiel met reviews, restitutieaanvraag voor ongeldige leads.

## Databasis

| bron | rijen (vakman) | opmerking |
|---|---|---|
| Google Play – Werkspot voor Vakmensen | 32 | 200 nieuwste reviews opgehaald (thewolves-scraper); inhoudsloze 1-woord-reviews ("goed", "oplichters") niet opgenomen; vooral 2024–2026 |
| App Store NL – Werkspot voor vakmensen | 23 | alle 93 opgehaald; selectie vanaf 2024 met inhoud |
| Trustpilot NL (www.werkspot.nl) | 48 | 262 NL-reviews 1–3 sterren sinds 1-11-2024 opgehaald; de **nieuwste 130 gelezen** (nov 2025 – okt 2026) en daaruit de vakmanreviews gecodeerd |
| Trustpilot EN | 12 | 187 Engelstalige reviews (alle sterren); gelezen t/m nov 2024 |
| Radar-forum (AVROTROS) | 3 | draad "Als zzp'er zwaar benadeeld door Werkspot" – **oud (2018–2019)**, alleen als achtergrond |
| **totaal vakman** | **118** | 99 van de 118 sinds nov 2024 |
| consument (apart, over vakman-opvolging) | 11 | Trustpilot NL/EN |

- **Verdeling vakmanrijen**: 1 ster 91 · midden 21 · positief 3 · zonder score 3 (forum).
- **Periode**: hoofdzakelijk nov 2024 – nov 2026; 16 rijen uit jan–okt 2024 (app-stores), 3 uit 2018–2019 (forum).
- **Kwaliteitsnoot**:
  - Sterke selectiebias: Trustpilot is bewust gefilterd op 1–3 sterren (om vakmanklachten te vinden tussen ~7.700 overwegend positieve consumentenreviews). De vakman-apps zijn ongefilterd, maar ook daar overheerst 1 ster; de paar 5-sterrenreviews zijn vaak inhoudsloos ("Top app"). Het beeld "vakmannen zijn ontevreden" is dus robuust, maar de *mate* is niet te kwantificeren.
  - Reviewer_type is bij app-store-reviews afgeleid uit de app (vakman-app) en inhoud; bij Trustpilot alleen als de tekst duidelijk vakman-signalen bevat ("als vakman", "leads", "zzp'er", "restitutie").
  - Niet opgehaald / niet gevonden: Kassa (BNNVARA) – geen uitzending/artikel specifiek over Werkspot-leadkosten gevonden; Reddit – geen relevante draden gevonden via zoeken; Tweakers en LinkedIn niet doorzocht (credit-zuinigheid). Directe toegang tot Radar-forum en werkspot.nl was vanuit de sandbox geblokkeerd; via Apify web-fetch opgehaald.
  - Restant van de Trustpilot-NL-dataset (132 reviews, nov 2024 – okt 2025) niet gelezen; titels tonen hetzelfde patroon ("Hoge leadkosten", "Leadkosten te hoog voor de vakman", "Begin er niet aan als vakman").

## Wat vakmannen goed vinden (de lat)

Waardering is dun en vrijwel altijd verpakt in kritiek:
- **Het concept / volume aan aanvragen**: "ik ben groot fan van het concept als het gaat om klanten te vinden" (Google Play, 2026-03-01, 2★); "Good company, plenty of jobs found here" (Trustpilot EN, 2024-11-27, 5★).
- **De app zelf werkt voor sommigen prima**: "app werk goed. kosten leadprijs zijn vaak wel hoog … 8 van de 10 klussen gaan door … Aantal revieuws en de 5* werkt uitstekend." (Google Play, 2025-05-30, 5★); "De app werkt goeg lead prijs is te hoog" (Google Play, 2025-10-24).
- **Reviews als verkoopinstrument**: opgebouwde reviews worden als waardevol gezien – juist daarom is verlies ervan (accountblokkade) zo pijnlijk.
- **Goedkoper dan zelf adverteren** (oud, 2018): "altijd goedkoper dan dat je zelf op google moet adverteren".

**Lat voor ons**: vakmannen willen een constante stroom aanvragen in hun vak/regio, een werkende chat/app en een reviewprofiel dat ze kunnen meenemen.

## Top 5 pijnpunten (vakmanrijen, n=118)

| # | thema | frequentie (1★ / midden / pos) | ernst |
|---|---|---|---|
| 1 | `leadkosten` – betalen per contact i.p.v. per opdracht, hoge/willekeurige prijzen | 93 (75 / 14 / 2) | zeer hoog – reden om te stoppen |
| 2 | `leadkwaliteit` – klant reageert niet, nep/onjuist nummer, alleen prijs-shoppen, slecht omschreven klus | 58 (52 / 6 / 0) | zeer hoog |
| 3 | `support` – restitutie standaard afgewezen, geen telefoon, robotmails, incasso | 42 (38 / 3 / 0) | hoog |
| 4 | `lead-concurrentie` – lead aan 5–10+ vakmannen verkocht, prijsstrijd | 20 (17 / 3 / 0) | hoog |
| 5 | `bugs`/`mobiel` – app crasht, uitloggen, berichten komen niet aan | 13 / 8 | middel |

Daarnaast: `lock-in` 9 (account geblokkeerd → reviews kwijt; opzeggen abonnement lukt niet), `onboarding` 3 (KvK-verificatie duurt weken).

**1. Leadkosten (betalen vóór er werk is)**
- "ik kan er vooral slecht tegen dat de leadprijs bij contact wordt verrekend in plaats van inhuur." (Google Play, 2026-03-01, 2★)
- "gemiddelde prijs per lead rond de €20 lag, dat is nu hedendaags €40 geworden." (Trustpilot NL, 2026-07-05, 1★)
- "Lead kosten per project zijn ook totaal niet goed bekeken, 11 € voor een plintje vervangen en 4€ voor 50m2 stucwerk." (Trustpilot NL, 2026-10-17, 1★)

**2. Leadkwaliteit**
- "9 van de 10 klanten die een chat starten zijn niet bereikbaar enof ze reageren niet/nooit!" (Trustpilot NL, 2026-07-05, 1★)
- "Klussen die per ongeluk geplaatst zijn. Klussen die maanden terug al zijn uitgevoerd. … En als ondernemer betaal je áltijd" (Trustpilot NL, 2025-11-24, 1★)
- "Reageer je op ‘complete badkamerrenovatie’ en betaal je de leadprijs om er achter te komen dat ze alleen een nieuwe douche willen." (App Store, 2025-05-31, 1★)

**3. Support / geld terug**
- "Klachten en restitutieverzoeken worden standaard afgewezen met copy-paste mails die enkel naar de voorwaarden verwijzen" (Google Play, 2025-09-18, 1★)
- "Ik heb gelukkig me geld terug gekregen, Nou ja het wordt in mindering gebracht op je volgende factuur." (Trustpilot NL, 2026-02-20, 1★)
- "factuur van ongeveer €200 gestuurd en deze direct overgedragen aan een incassobureau." (Trustpilot NL, 2025-11-21, 1★)

**4. Concurrentie per lead**
- "Je concurreert al snel met 5  andere vakmensen. Echter betaalt elke vakman de volle mep om te mogen concurreren. 20 tot 40 euro!!" (App Store, 2024-12-24, 1★)
- "10 klussers zijn aangevinkt … Dan betalen alle 10 klussers 12,- terwijl de klant maar 1 voor klusser kiest." (App Store, 2024-07-01, 2★)
- "ZOEK EEN ANDER PLATFORM … WAAR ELKE KLUS NAAR MAXIMAAL 3 TOT 4 MAN WORDT VERZONDEN" (Trustpilot NL, 2026-02-18, 1★)

**5. App / lead-opvang technisch**
- "app moet 3 of 4 keer per maand opnieuw geïnstalleerd worden om überhaupt te functioneren." (Google Play, 2026-04-19, 2★)
- "Berichten komen niet goed aan, reviews niet te bekijken en wijzigingen komen niet altijd door." (Google Play, 2024-03-04, 2★)

## "Wat net mist" (middenreviews, n=21)

- **Het model is acceptabel, de verhouding niet.** Middenreviewers accepteren betalen voor leads ("Op zich geen slecht model" – Trustpilot NL 2026-02-07, 2★; "Ik snap dat ze een bedrag in rekening brengen" – 2026-03-22, 2★), maar willen dat de prijs past bij de klusgrootte en dat betalen pas bij een echte opdracht/wederzijdse bevestiging gebeurt. "Naarmate je als bedrijf/vakman groeit zal je derhalve werkspot willen verlaten."
- **Aanvragen zijn te vaag om te kunnen prijzen.** "opdrachten zijn vaak niet goed omschreven. Er is een verschil tussen een Beton en een afwerkvloer" (Google Play, 2024-09-08, 4★). De beveiligingsinstallateur (2026-09-05) vraagt eerst foto's en betaalt al voordat hij weet wat er nodig is.
- **Transparantie naar de consument ontbreekt.** Meerdere vakmannen zetten zelf onder elk bericht dat reageren hen geld kost; zij willen dat het platform de consument dit vertelt.
- **App-basics**: na updates kun je niet terug naar overzicht, interesses opnieuw invoeren (App Store 2024-02-23, 3★); foutmeldingen (Google Play 2025-08-04, 4★).
- **Restitutie kan wél werken, maar traag**: "inmiddels opgelost duurde wel heel lang maar de €50 is niet in rekening gebracht!" (Trustpilot NL, 2026-08-28, 3★).

Consumentenkant (11 rijen, apart geteld) bevestigt het effect: "ik steeds 10 bedrijven aanschrijf, maar dat ik steeds maar van 1 bedrijf een reactie krijg" (2026-10-08); "Bij en wat kleinere klus word er door bijna niemand gereageerd" (2026-08-08); en opvolging door vakmannen faalt: offerte nooit gestuurd na opmeten (2026-04-02), na ketelinstallatie "reageert hij niet meer om de ketel te onderhouden" (2025-11-25).

## Kansen voor ons CRM

1. **Lead-opvang + leadkosten-administratie**: vakmannen houden zelf niet bij wat een lead kostte en wat die opleverde. Een CRM dat leads uit Werkspot (mail/app-notificatie) automatisch binnenhaalt, de leadprijs vastlegt en per platform **kosten per gewonnen opdracht** berekent, geeft precies het inzicht waar deze reviewers zelf over rekenen ("1 klus uit 13 … €189 aan leads"). Ook bewijs verzamelen voor restitutie (niet-werkend nummer, geen reactie binnen X dagen) is een concrete feature.
2. **Snelle eerste reactie + kwalificatie**: omdat 5–10 vakmannen dezelfde lead krijgen, wint snelheid. Templates voor eerste reactie (incl. uurtarief/prijsindicatie en de kwalificatievragen + foto-verzoek), en een WhatsApp-vervolg zodra het nummer binnen is.
3. **Opvolgritme voor leads die "verdwijnen"**: Werkspot adviseert zelf meerdere pogingen over ongeveer een week; een automatische belpoging-/WhatsApp-/mailreeks met logging is direct nuttig (en levert bewijs voor restitutie).
4. **Offerte-opvolging**: consumentenreviews laten zien dat vakmannen offertes na opname niet versturen of opvolgen – herinneringen en status per aanvraag dichten dat gat.
5. **Eigen klantdossier en reviews los van het platform**: accountblokkades betekenen "na jaren … al mijn contacten kwijt en recensies". Een CRM waarin klanten, adressen en (eigen) reviews van de vakman zelf blijven, plus nazorg/onderhoudsherinneringen om herhaalwerk direct (zonder leadkosten) binnen te halen, is een sterk verkoopargument: minder afhankelijk van betaalde leads.
