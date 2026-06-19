# Roadmap — Conversion Gap Scan til 10 betalende kunder
## The Engines Behind / NorthLogicLab
### v2 — 2026-06-19 · Tidsbudget: ~10 timer/uge

---

## Hvad der er nyt i v2

Instrumentporteføljen har fået en klar funktionel logik den manglede i v1:

**Positionsanalysen = diagnosen (as-is).** Findes nu i to niveauer:
- **Individ** — "Hvad sker der med dit arbejde?" Gratis, selvbetjent, viralt. Driver trafik og data.
- **Organisation** — aggregering af individ-data til et organisatorisk eksponeringskort. Det HR/leder reelt skal se for at handle. Lav pris eller gratis som døråbner.

**Kapabilitetskortet** (tidligere "Rekrutteringsværktøjet") = løsningen (to-be). Bredere end navnet "rekruttering" antydede — det er det organisatoriske kapabilitetsbillede der driver fire forskellige beslutninger:
- Rekruttering (ekstern — hvad skal vi hente ind)
- Udvikling (intern — hvad skal vi opbygge)
- Succession planning (hvem er klar til hvad)
- Teamdesign (hvordan sammensætter vi det rigtigt)

Det er det betalte produkt. Det kræver organisatorisk arbejde at levere (ESCO-mapping, gap-analyse, anbefalinger) — det er derfor det er det der fakturerer.

**Den opdaterede tragt:**

```
Positionsanalysen (Individ)
   — gratis, viralt, leads, data til bogen
       ↓
Positionsanalysen (Organisation)
   — aggregeret billede, HR/leder-indgang
   — AS-IS er komplet på organisationsniveau
       ↓
Kapabilitetskortet
   — TO-BE: ESCO-gap identificeret
   — Fire anvendelser: rekruttering / udvikling / succession / teamdesign
       ↓
BETALT PRODUKT
```

---

## Præmis (uændret fra v1)

- **10 timer/uge.** Alt der ikke direkte fremmer næste milepæl, venter.
- **Danpo er døråbneren.** Succes med Danpo er forudsætningen for at nå Kronfågel, Den Stolte Hane, Manor Farm — ikke en sideeffekt.
- **Målet er 10 betalende kunder til Kapabilitetskortet.** Ikke 10 besvarelser. Ikke 10 samtaler. Penge på bordet.

---

## Fase 0 — Fundamentet (uge 1-2, ~20 timer)

**Hvad:** Gør begge niveauer af Positionsanalysen og Kapabilitetskortet klar til at producere data du kan bruge som bevis — og til at aggregere korrekt fra individ til organisation.

**Hvorfor:** Du kan ikke levere et organisatorisk billede til Danpo's HR-partner hvis individ-besvarelserne ikke er bygget til at rulle op i en aggregering fra dag ét. Dette er den tekniske detalje der er let at overse nu og dyr at rette bagefter.

**Konkret:**
1. **Positionsanalysen (Individ):** Tilføj `window.storage` — gem (anonymiseret) score, zone, branche og **et organisations-id/team-tag** per besvarelse, shared:true. Organisations-tagget er det nye — uden det kan du ikke bygge niveau 2.
2. **Positionsanalysen (Organisation):** Byg den aggregerende visning — tager alle besvarelser med samme organisations-tag og viser fordelingen på zoner. Kan være simpelt i v1: et antal og en procentfordeling, ikke et fancy dashboard.
3. **Kapabilitetskortet:** Tilføj samme dataopsamlingslag — hvilke arketyper identificeres, hvilke ESCO-gaps er mest udbredte
4. **Ét simpelt admin-view** (en markdown-rapport du genererer manuelt hver uge er fint) der viser: antal individ-besvarelser, antal organisationer repræsenteret, fordeling på zoner og arketyper

**Beslutningspunkt ved afslutning:** Kan du, givet et organisations-tag, generere et aggregeret billede uden manuelt at samle data fra enkeltbesvarelser? Hvis nej — stop her til det er løst. Det er forudsætningen for hele Fase 1.

---

## Fase 1 — Danpo som pilot (uge 3-6, ~40 timer)

**Hvad:** HR-partneren hos Danpo bruger Positionsanalysen (Individ) på en defineret gruppe. Du leverer Positionsanalysen (Organisation) som det aggregerede resultat. De mest relevante profiler får tilbudt Kapabilitetskortet.

**Hvorfor:** Danpo er ikke målet. Danpo er beviset der låser resten af Scandi op. Du har allerede adgangen — det der mangler er en struktur der gør testen til noget du kan vise frem.

**Konkret:**
1. **Aftal scope skriftligt med HR-partneren:** hvilken afdeling/gruppe (anbefaling: 15-30 personer), hvilken tidsramme (2 uger)
2. **Kør Positionsanalysen (Individ) først** — lavfriktion, ingen "godkendelse" nødvendig for at deltage, alle får et personligt resultat med det samme
3. **Lever Positionsanalysen (Organisation) til HR-partneren** efter 2 uger — det aggregerede billede af hele gruppen. Dette er det første reelle leverancepunkt
4. **Tilbyd Kapabilitetskortet til de 3-5 mest relevante profiler/funktioner** identificeret via det organisatoriske billede — typisk hvor zonen er højest eller hvor en kritisk rolle viser eksponering
5. **Lav ÉN strukturerede tilbagemelding** — ikke 20 sider. Tre ting: (a) hvad det organisatoriske billede viste, (b) hvad det betyder konkret for Danpo, (c) hvad de kan gøre via Kapabilitetskortets fire anvendelser

**Det kritiske krav du skal stille til Danpo (sig det direkte, tidligt):**
"Positionsanalysen er gratis. Betalingen er at jeg kan bruge anonymiserede aggregerede data — ikke navne, ikke specifikke svar — som bevis for at det virker, internt i Scandi og eksternt i bogen."

Hvis de siger nej til det, har du en tjeneste, ikke en case. Få det aftalt før I starter.

**Beslutningspunkt ved afslutning:** Har du et organisatorisk tal du kan vise frem? Eksempel: *"73% af Danpo's [afdeling] scorer i moderat-til-høj eksponering, men kun 1 ud af 12 har en Oversætter-profil."* Konverterede mindst én relevant profil til en betalt Kapabilitetskort-session? Hvis ikke — undersøg om det er fordi billedet ikke var skarpt nok, eller fordi prisen/produktet ikke landede, inden du går videre.

---

## Fase 2 — Det interne salg i Scandi (uge 7-9, ~20 timer)

**Hvad:** Brug Danpo's organisatoriske resultat til at åbne Kronfågel, Den Stolte Hane og Manor Farm.

**Hvorfor:** Det er her "Scandi som laboratorium" reelt betaler sig. Du har relationen via koncernen — det du mangler er beviset, og det har du nu.

**Konkret:**
1. **Skriv ét ark** — ikke en pitch deck — der viser Danpo's organisatoriske billede (Positionsanalysen niveau 2) og spørger: "Vil I have det samme billede af jeres organisation?"
2. **Send direkte til HR/procurement-ledere** i de øvrige Business Units — brug Danpo-kontakten som reference
3. **Samme to-trins model:** gratis Positionsanalyse (begge niveauer), betalt Kapabilitetskort for de der vil gå fra diagnose til handling

**Beslutningspunkt ved afslutning:** Har mindst én Business Unit udover Danpo betalt for Kapabilitetskortet? Hvis ja — du har bevis at modellen skalerer internt, gå til Fase 3. Hvis nej — undersøg hvorfor inden du går eksternt.

---

## Fase 3 — Ekstern outreach (uge 10-14, ~40 timer)

**Hvad:** Direkte outreach til procurement/HR-ledere udenfor Scandi-koncernen, baseret på de interne cases.

**Hvorfor:** Du har nu et navngivet problem (Conversion Gap), et bevisbart instrument (Positionsanalysen, to niveauer) og et internt bevis for at det konverterer til betaling (Scandi-data).

**Konkret:**
1. **Skriv ét outreach-skema:** "Jeg arbejder på Conversion Gap — gabet mellem adgang og kapabilitet. Vi har testet det internt i Scandi [konkret tal]. Vil I tage en 20-minutters gratis Positionsanalyse?"
2. **Mål: 30-40 henvendelser per uge** til procurement-/HR-ledere i tilsvarende brancher (food & beverage, fragmenterede forsyningskæder, regulatorisk tung industri)
3. **Positionsanalysen (Individ) er den eneste "salgssamtale" du behøver i første kontakt**
4. **Opfølgning med Positionsanalysen (Organisation) kun til dem der får flere kolleger til at deltage** — det er det signal der viser reel organisatorisk interesse, ikke blot personlig nysgerrighed
5. **Kapabilitetskortet tilbydes når organisationsbilledet er klart**

**Beslutningspunkt ved afslutning:** Hvor mange eksterne organisationer konverterede fra individ-besvarelse → organisationsbillede → betalt Kapabilitetskort? Det er din reelle konverteringsrate gennem hele tragten — brug den til at regne baglæns hvor mange henvendelser de sidste kunder kræver.

---

## Fase 4 — Skalering mod 10 (løbende, resten af tidsbudgettet)

**Hvad:** Gentag Fase 3's mekanisme med justeringer baseret på hvor tragten faktisk lækker.

**Hvorfor:** Ved dette punkt har du data nok til at vide om flaskehalsen er **leads** (for få besvarer Positionsanalysen Individ), **organisatorisk konvertering** (mange individer besvarer, men ingen samler en gruppe til niveau 2), eller **produkt/pris** (organisationsbilledet er klart, men de siger nej til Kapabilitetskortet).

**Tre forskellige justeringer afhængig af hvad du ser:**

- **Hvis problemet er leads til Individ-niveauet:** Brug Danpo/Scandi-casen som indhold — et kort LinkedIn-opslag der linker direkte til Positionsanalysen
- **Hvis problemet er konvertering fra Individ til Organisation:** Det betyder folk tager testen for egen nysgerrighed, men ingen samler kolleger om det. Overvej om HR/leder skal være indgangen fra start i den eksterne outreach, ikke individet
- **Hvis problemet er Kapabilitetskortets pris/produkt:** Det vigtigste signal — organisationer anerkender gabet, men ikke nok til at betale endnu. Det er et produktspørgsmål: er de fire anvendelser (rekruttering/udvikling/succession/teamdesign) tydelige nok i hvad de reelt får?

**Beslutningspunkt:** Ved 10 betalende kunder til Kapabilitetskortet er roadmap'et fuldført. Herfra handler det om pris-optimering, et lettere onboarding-flow, og brug af den aggregerede data i bogens Akt 3.

---

## Hvad der eksplicit IKKE er i dette roadmap

- Markedsføring af bogen som selvstændigt produkt
- Yderligere udvikling af Karrierekompas/Selvdiagnostik udover det der direkte støtter salgsflowet
- Konkurrentanalyse — relevant senere, ikke nu
- Detaljeret prisstrategi for Kapabilitetskortet — sæt en pris, test den, juster baseret på faktiske reaktioner i Fase 1-3

---

## Sammenfattet tidslinje

| Fase | Uger | Timer | Output |
|---|---|---|---|
| 0 — Fundament (to-niveau dataopsamling) | 1-2 | 20 | Aggregering individ→organisation virker |
| 1 — Danpo pilot | 3-6 | 40 | Ét bevisbart organisatorisk tal + 1. betalingssignal |
| 2 — Internt Scandi-salg | 7-9 | 20 | 1+ betalende BU internt |
| 3 — Ekstern outreach | 10-14 | 40 | Konverteringsrate gennem hele tragten kendt |
| 4 — Skalering | 15+ | Løbende | 10 betalende kunder til Kapabilitetskortet |

**Samlet til første bevisbare resultat (Fase 0+1): ~6 uger, ~60 timer.**
**Samlet til 10 betalende kunder: realistisk 4-6 måneder ved 10 timer/uge.**

---

## Navngivning — opsummeret

| Gammelt navn | Nyt navn | Funktion |
|---|---|---|
| Skæbnescenariet / Positionsanalysen | **Positionsanalysen — Individ** | AS-IS, personligt niveau |
| (ny) | **Positionsanalysen — Organisation** | AS-IS, aggregeret organisationsniveau |
| Rekrutteringsværktøjet | **Kapabilitetskortet** | TO-BE, betalt, fire anvendelser |

---

*Roadmap v2 — The Engines Behind / NorthLogicLab*
*Bygget til at blive justeret efter Fase 1's faktiske resultat — ikke en statisk plan.*

