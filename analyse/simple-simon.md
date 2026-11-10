# Simple-Simon – review-analyse

## Profielschets

- **Wat**: werkbon- en planningsapp ("De Slimme Werkbon") uit Eindhoven, voor mkb en zzp. Er is een backoffice/console met grafisch planbord en een mobiele app (Android `com.mobileop`, iOS id897884395). Ruim 50.000 Android-installaties (AppBrain, via WebSearch).
- **Doelgroep (uit reviews)**: installateurs, deur- en aluminiumtechniek, hoveniers, onderhoudsbedrijven met meerdere monteurs (bv. "klein bedrijf met 12 monteurs"), ook Belgische bedrijven.
- **Kernfuncties**: digitale werkbon (uren, materialen via barcode, foto's, pdf, handtekening), eigen formulieren/keuringsformulieren en checklists, eigen werkbonlayout, planbord met herhalende afspraken en roosters, objecten per werkadres (sinds v2.0, 2019), voorraadbeheer, automatische mail naar de klant. Volgens de App Store-beschrijving online en offline. Koppelingen met Exact Online, SnelStart, AFAS, MS Dynamics BC, Informer, easybill en API's.
- **Prijsindicatie**: **niet opgehaald**. De fetch van simple-simon.nl/prijzen liep uit op een timeout (60 s) en WebSearch vond geen prijspagina. De App Store noemt alleen 14 dagen gratis proberen zonder creditcard. Uit reviews: "niet duur voor alle opties" (aug 2026), "per maand het aantal gebruikers kunt instellen" (jun 2022), maar ook "Behoorlijk duur ook om een abonnement te nemen" (sep 2021).

## Databasis

| bron | opgehaald | in CSV | waarvan sinds nov 2024 |
|---|---|---|---|
| Google Play (com.mobileop, NL, NEWEST, max 100) | 100 | 28 | 7 |
| App Store NL (id897884395, max 100) | 100 | 37 | 5 |
| **Totaal** | 200 | **65** | **12** |

- **Selectie**: alle reviews vanaf 2022 zijn opgenomen (twee nietszeggende/spam-reviews weggelaten). Van vóór 2022 zijn alleen de kritische reviews opgenomen, plus twee informatieve positieve (klein bedrijf met 12 monteurs; automatische klantmails). Daardoor zijn de pijnpunten in de CSV relatief oververtegenwoordigd ten opzichte van de ruwe data: de ruwe 200 zijn nog positiever.
- **Verdeling CSV**: 9 × 1 ster, 10 × midden, 46 × positief. Groepsregel: 4–5 sterren met een klachtcode tellen als midden.
- **Periode**: nov 2018 – aug 2026. Slechts 12 reviews vallen in de laatste 24 maanden (2 × 1 ster, 1 midden, 9 positief).
- **Kwaliteitsnoot (belangrijk)**:
  - **De data is dun en waarschijnlijk positief gekleurd.** Tientallen 5-sterrenreviews uit 2019–2020 gaan over "goede training van Hadiya" en zijn kennelijk direct na een training geplaatst. Eén 1-sterreview (App Store, apr 2019) zegt: "recensies worden min of meer gedwongen bij uitleg."
  - Er is weinig bruikbare kritiek. Conclusies over pijnpunten rusten op 19 rijen, en die zijn grotendeels ouder dan 2 jaar.
  - Trustpilot (simple-simon.nl): geen profiel gevonden (actor: "profile not found"). Een alternatief domein vond ik niet via WebSearch.
  - G2: volgens WebSearch 1 review (2023, uitgenodigd); niet opgehaald.
  - Capterra/GetApp: geen profiel gevonden.
  - Google Maps, Tweakers en Reddit: niet geprobeerd. Dat is bewust, om credits te sparen; er waren geen aanwijzingen voor klantreviews daar.

## Wat gebruikers goed vinden (de lat)

- **Eenvoud, ook voor monteurs**: "Zoals de naam het al zegt Simpel, maar heel erg fijn en professioneel in gebruik" (Play, dec 2021, 12 monteurs). "na een paar uurtjes uitzoek werk kon ik makkelijk zonder enige training mijn collega’s op pad sturen" (App Store, nov 2022).
- **Support is bereikbaar, ook telefonisch**: 12 positieve vermeldingen. "Bij problemen is de support afdeling gemakkelijk te bereiken, ook telefonisch!" (App Store, nov 2023).
- **Onderhoud en historie per object**: "Periodiek onderhoud aan machines is gemakkelijk in te plannen, met voorraad beheer, opvolging, geschiedenis gemakkelijk te bekijken voor de monteurs onderweg" (App Store, nov 2023). "automatisch een dossier opbouwen" (App Store, nov 2022).
- **Zelf in te richten formulieren en layouts**: "eigen keuringsformulieren voor onze installaties" (App Store, feb 2023).
- **Realtime status naar kantoor en klant**: "geeft real time door wat de status is van een opdracht" (Play, dec 2023). "mailtjes worden automatisch naar de klant verstuurd" (App Store, jun 2020).
- **Boekhoudkoppeling** (Exact, SnelStart, AFAS): 5 positieve vermeldingen.
- **Flexibel prijsmodel**: gebruikers per maand aan te passen.

## Top 5 pijnpunten

Dun: in totaal 19 rijen met een klacht, waarvan maar 3 uit de laatste 24 maanden.

| # | thema | frequentie (van 65) | 1 ster / midden | ernst |
|---|---|---|---|---|
| 1 | mobiele app (inloggen, kleine velden, geen meldingen, toestemmingen) | 7 | 5 / 2 | middel |
| 2 | bugs / traagheid / vastlopen na updates | 6 | 4 / 2 | middel (meestal oud: 2019–2020) |
| 3 | werkbon-invoer omslachtig of beperkt (klikken, decimalen, layout) | 5 | 2 / 3 | middel |
| 4 | gebruiksgemak (niet intuïtief, "druk") | 4 | 2 / 2 | middel |
| 5 | support via e-mail traag / niet telefonisch | 3 | 3 / 0 | middel (tegenover 12 positieve vermeldingen) |

**1. Mobiel**
- "inloggen zeer moeilijk? blijft resetten" (Play, 2025-07-11, 1★)
- "niet altijd even smartphone vriendelijk. Invulvelden zijn veel te klein. Krijg géén meldingen bij een gewijzigde planning" (Play, 2021-09-23, 3★)

**2. Bugs**
- "vol met bugs, natuurlijk tijdverloop bestaat niet, aanpassingen zijn vrijwel onmogelijk" (Play, 2025-06-09, 1★, monteur)
- "Vrij irritante bugs, toetsenbord kan niet geannuleerd worden" (App Store, 2020-08-13, 3★)

**3. Werkbon-invoer**
- "veelste veel klikken … Kost teveel tijd..." (App Store, 2019-07-04, 2★)
- "Helaas is het niet mogelijk om met decimalen te werken in de aantallen" (App Store, 2019-01-31, 4★)
- "de opmaakmogelijkheden voor de werkbonlayout wat beperkt" (Play, 2022-02-15, 4★)

**4. Gebruiksgemak**
- "totaal niet intuitief in gebruik … ik ga fijn terug naar papieren bon!" (Play, 2025-06-09, 1★)
- "Keurige app, wel wat druk" (App Store, 2019-12-30, 4★)

**5. Support**
- "heen en weer mailen duurt veel te lang" (Play, 2025-06-09, 1★)
- "na het keuze menu waarbij je kiest voor support word je verzogd om een mail te sturen" (Play, 2019-06-19, 1★)

## "Wat net mist" (middenreviews, n=10)

- **Koppelingen zijn er, maar net niet volledig**: "Koppeling SnelStart is enigszins beperkt, individuele prijsafspraken worden niet meegenomen" (2020). "zien we graag nog wat extra gegevens gesynchroniseerd" (MS Dynamics, 2022). "Koppeling met SnelStart had wat voeten in de aarde" (2019).
- **Meldingen en planning-sync naar de monteur**: er komt geen pushmelding bij een gewijzigde planning (2021). Gebruikers wachten op een "jaarplanning", wat relevant is voor periodiek onderhoud (2022).
- **Kleine invoerdetails in het veld**: decimalen, kleine invulvelden en het aantal klikken per bon.
- **Recent** alleen: "heeft nog wel wat verbeteringen nodig" (Play, aug 2026, 3★), zonder details.

## Kansen voor ons CRM

1. **Simple-Simon is een sterke lat voor eenvoud en support.** Een concurrent met minder bugs en goede telefonische support moet je niet aanvallen op werkbon/planning alleen. De kans zit in wat Simple-Simon niet doet.
2. **Lead-opvang en offerte-opvolging**: komen in geen enkele review voor. Simple-Simon begint bij de werkbon/opdracht, dus de aanvraag- en offertefase (WhatsApp, mail, leadplatforms) ervóór is open terrein. Let op: dit volgt uit afwezigheid in de reviews, niet uit expliciete klachten.
3. **Onderhoudscontracten en jaarplanning**: periodiek onderhoud en objecthistorie worden gewaardeerd, maar de jaarplanning werd nog gemist (2022). Automatisch terugkerende onderhoudsafspraken per adres/object, met klantherinnering via WhatsApp, past hierbij.
4. **Klantcommunicatie**: automatische mails naar de klant worden gewaardeerd (2020). WhatsApp-statusupdates ("monteur onderweg", werkbon met handtekening) zijn een logische stap verder.
5. **Pushmeldingen bij planningswijzigingen** en kleine invoerdetails (decimalen, grote invoervelden) als basisniveau.
6. **Review-integriteit**: de gestuurde reviews na trainingen maken de app-store-score onbetrouwbaar als benchmark. Voor eigen marktonderzoek bij overstappers zijn diepte-interviews met Simple-Simon-gebruikers nodig.
