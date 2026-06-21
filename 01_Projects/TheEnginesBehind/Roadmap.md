# Roadmap — Conversion Gap Scan til 10 betalende kunder
## The Engines Behind / NorthLogicLab
### v4 — 2026-06-21 · Tidsbudget: ~10 timer/uge

---

## Hvad der er nyt i v4

To rettelser, begge fordi roadmap-teksten ikke længere matchede de faktisk byggede filer.

**Strukturen er tre niveauer, ikke to.** De faktiske filnavne i repoet er `Positionsanalyse_individ.html`, `Positionsanalyse_Org_individ.html` og `Positionsanalyse_Org_Org.html` — tre separate instrumenter, ikke "Individ" og "Organisation" som tidligere beskrevet. `Org_individ` er det HR sender internt til medarbejdere for at indsamle AS-IS-data med et organisations-tag. `Org_Org` er det aggregerede dashboard der summerer alle `Org_individ`-besvarelser med samme tag til ét organisatorisk billede. Det er ikke en omskrivning af mekanismen — det er en korrektion af navngivningen, så roadmap'en matcher koden.

**Kapabilitetskortet har seks anvendelser, ikke fire.** De faktiske faner i `Kapabilitetskortet.html` er: ACA-analyse (rekruttering), Udvikling, Succession & Teamdesign, Interviewspørgsmål, Stillingsopslag og Skjulte talenter. De sidste tre var allerede bygget, men ikke navngivet i roadmap-teksten. Se opdateret tragt-diagram nedenfor.

---

## Hvad der var nyt i v3

Capability Stack Analysis og Capability Position Scorecard tilføjet som eksplicit udskudte, fremtidige produktmuligheder — se afsnit efter "Hvad der eksplicit IKKE er i dette roadmap".

---

## Hvad der var nyt i v2

Instrumentporteføljen har fået en klar funktionel logik den manglede i v1:

**Positionsanalysen = diagnosen (as-is).** Findes i tre niveauer:
- **Individ** (`Positionsanalyse_individ.html`) — "Hvad akkumulerer dit arbejde?" Gratis, selvbetjent, viralt. Driver trafik og data til bogen. Ingen organisatorisk kontekst.
- **Organisation–individ** (`Positionsanalyse_Org_individ.html`) — samme spørgsmål, men med et organisations-tag. Det HR sender internt til en defineret medarbejdergruppe for at afdække AS-IS på individniveau, klar til aggregering.
- **Organisation–org** (`Positionsanalyse_Org_Org.html`) — "Hvilke kapabiliteter mangler I — og hvor er jeres største risici?" Det aggregerede dashboard. Summerer alle Organisation–individ-besvarelser med samme tag til ét organisatorisk billede. Det er HR/leder-indgangen, og det er her AS-IS er komplet på organisationsniveau.

**Kapabilitetskortet** (tidligere "Rekrutteringsværktøjet") = løsningen (to-be). Bredere end navnet "rekruttering" antydede — det er det organisatoriske kapabilitetsbillede der driver seks forskellige anvendelser:
- **ACA-analyse / rekruttering** (ekstern — hvad skal vi hente ind)
- **Udvikling** (intern — hvad skal vi opbygge)
- **Succession & Teamdesign** (hvem er klar til hvad, hvordan sammensætter vi det rigtigt)
- **Interviewspørgsmål** (operationaliserede spørgsmål til selve samtalen — bygger på samme EPOCH-baserede logik som rekrutteringskapitlet i bogen)
- **Stillingsopslag** (omsætter ACA-profilen direkte til en jobannonce)
- **Skjulte talenter** (identificerer høj-ACA-profiler der ikke er synlige i den traditionelle talentpulje — bogens "skjulte talent-paradoks" gjort til et værktøj)

Det er det betalte produkt. Det kræver organisatorisk arbejde at levere (ESCO-mapping, gap-analyse, anbefalinger) — det er derfor det er det der fakturerer.

**Den opdaterede tragt:**

```
Positionsanalysen — Individ
   — gratis, viralt, leads, data til bogen
       ↓
Positionsanalysen — Organisation–individ
   — HR sender internt til medarbejdergruppe
   — afdækker AS-IS på individniveau
       ↓
Positionsanalysen — Organisation–org
   — aggregeret billede, HR/leder-indgang
   — AS-IS er komplet på organisationsniveau
       ↓
Kapabilitetskortet
   — TO-BE: ESCO-gap identificeret
   — Seks anvendelser: rekruttering / udvikling / succession & teamdesign /
     interviewspørgsmål / stillingsopslag / skjulte talenter
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

**Hvad:** Gør alle tre niveauer af Positionsanalysen og Kapabilitetskortet klar til at producere data du kan bruge som bevis — og bekræft at aggregeringen fra Organisation–individ til Organisation–org rent faktisk virker i praksis, ikke kun i koden.

**Hvorfor:** Du kan ikke levere et organisatorisk billede til Danpo's HR-partner hvis individ-besvarelserne ikke ruller korrekt op i aggregeringen. `Positionsanalyse_Org_individ.html` gemmer allerede besvarelser under `pos-individ:`-nøgler, og `Positionsanalyse_Org_Org.html` læser dem allerede via et `pos-org-index`. Det tekniske lag er bygget — det der mangler er at bekræfte det virker med rigtige data, ikke at bygge det fra bunden.

**Konkret:**
1. **Positionsanalysen — Organisation–individ:** Bekræft at `window.storage` gemmer (anonymiseret) score, zone, branche og organisations-tag korrekt per besvarelse, shared:true.
2. **Positionsanalysen — Organisation–org:** Test den aggregerende visning med et testdatasæt (5-10 fiktive besvarelser under samme organisations-tag) — bekræft fordelingen på zoner vises korrekt, før den bruges på rigtige Danpo-data.
3. **Positionsanalysen — Individ:** Bekræft den forbliver uden organisatorisk kontekst — det er den rene, virale indgang, og skal ikke kræve et tag.
4. **Kapabilitetskortet:** Tilføj et dataopsamlingslag — hvilke arketyper identificeres, hvilke ESCO-gaps er mest udbredte, og hvilke af de seks faner (analyse/udvikling/succession/interview/opslag/talent) der reelt bliver brugt
5. **Ét simpelt admin-view** (en markdown-rapport du genererer manuelt hver uge er fint) der viser: antal individ-besvarelser, antal organisationer repræsenteret, fordeling på zoner og arketyper

**Beslutningspunkt ved afslutning:** Kan du, givet et organisations-tag, generere et aggregeret billede via Organisation–org uden manuelt at samle data fra enkeltbesvarelser? Hvis nej — stop her til det er løst. Det er forudsætningen for hele Fase 1.

---

## Fase 1 — Danpo som pilot (uge 3-6, ~40 timer)

**Hvad:** HR-partneren hos Danpo bruger Positionsanalysen — Organisation–individ på en defineret gruppe. Du leverer Positionsanalysen — Organisation–org som det aggregerede resultat. De mest relevante profiler får tilbudt Kapabilitetskortet.

**Hvorfor:** Danpo er ikke målet. Danpo er beviset der låser resten af Scandi op. Du har allerede adgangen — det der mangler er en struktur der gør testen til noget du kan vise frem.

**Konkret:**
1. **Aftal scope skriftligt med HR-partneren:** hvilken afdeling/gruppe (anbefaling: 15-30 personer), hvilken tidsramme (2 uger)
2. **Kør Positionsanalysen — Organisation–individ først, med Danpo's organisations-tag** — lavfriktion, ingen "godkendelse" nødvendig for at deltage, alle får et personligt resultat med det samme. Det skal være Organisation–individ, ikke det rene, tag-løse Individ-instrument — ellers kan besvarelserne ikke aggregeres i næste trin.
3. **Lever Positionsanalysen — Organisation–org til HR-partneren** efter 2 uger — det aggregerede billede af hele gruppen. Dette er det første reelle leverancepunkt
4. **Tilbyd Kapabilitetskortet til de 3-5 mest relevante profiler/funktioner** identificeret via det organisatoriske billede — typisk hvor zonen er højest eller hvor en kritisk rolle viser eksponering
5. **Lav ÉN strukturerede tilbagemelding** — ikke 20 sider. Tre ting: (a) hvad det organisatoriske billede viste, (b) hvad det betyder konkret for Danpo, (c) hvad de kan gøre via Kapabilitetskortets seks anvendelser

**Det kritiske krav du skal stille til Danpo (sig det direkte, tidligt):**
"Positionsanalysen er gratis. Betalingen er at jeg kan bruge anonymiserede aggregerede data — ikke navne, ikke specifikke svar — som bevis for at det virker, internt i Scandi og eksternt i bogen."

Hvis de siger nej til det, har du en tjeneste, ikke en case. Få det aftalt før I starter.

**Beslutningspunkt ved afslutning:** Har du et organisatorisk tal du kan vise frem? Eksempel: *"73% af Danpo's [afdeling] scorer i moderat-til-høj eksponering, men kun 1 ud af 12 har en Oversætter-profil."* Konverterede mindst én relevant profil til en betalt Kapabilitetskort-session? Hvis ikke — undersøg om det er fordi billedet ikke var skarpt nok, eller fordi prisen/produktet ikke landede, inden du går videre.

---

## Fase 2 — Det interne salg i Scandi (uge 7-9, ~20 timer)

**Hvad:** Brug Danpo's organisatoriske resultat til at åbne Kronfågel, Den Stolte Hane og Manor Farm.

**Hvorfor:** Det er her "Scandi som laboratorium" reelt betaler sig. Du har relationen via koncernen — det du mangler er beviset, og det har du nu.

**Konkret:**
1. **Skriv ét ark** — ikke en pitch deck — der viser Danpo's organisatoriske billede (Positionsanalysen — Organisation–org) og spørger: "Vil I have det samme billede af jeres organisation?"
2. **Send direkte til HR/procurement-ledere** i de øvrige Business Units — brug Danpo-kontakten som reference
3. **Samme tre-trins model:** gratis Positionsanalyse (Organisation–individ → Organisation–org), betalt Kapabilitetskort for de der vil gå fra diagnose til handling

**Beslutningspunkt ved afslutning:** Har mindst én Business Unit udover Danpo betalt for Kapabilitetskortet? Hvis ja — du har bevis at modellen skalerer internt, gå til Fase 3. Hvis nej — undersøg hvorfor inden du går eksternt.

---

## Fase 3 — Ekstern outreach (uge 10-14, ~40 timer)

**Hvad:** Direkte outreach til procurement/HR-ledere udenfor Scandi-koncernen, baseret på de interne cases.

**Hvorfor:** Du har nu et navngivet problem (Conversion Gap), et bevisbart instrument (Positionsanalysen, tre niveauer) og et internt bevis for at det konverterer til betaling (Scandi-data).

**Konkret:**
1. **Skriv ét outreach-skema:** "Jeg arbejder på Conversion Gap — gabet mellem adgang og kapabilitet. Vi har testet det internt i Scandi [konkret tal]. Vil I tage en 20-minutters gratis Positionsanalyse?"
2. **Mål: 30-40 henvendelser per uge** til procurement-/HR-ledere i tilsvarende brancher (food & beverage, fragmenterede forsyningskæder, regulatorisk tung industri)
3. **Positionsanalysen — Individ (den rene, tag-løse version) er den eneste "salgssamtale" du behøver i første kontakt** — ingen organisatorisk binding endnu, lavest mulig friktion for en kold kontakt
4. **Når flere kolleger fra samme organisation melder sig, skift til Organisation–individ med et tag, og lever Organisation–org som opfølgning** — det er det signal der viser reel organisatorisk interesse, ikke blot personlig nysgerrighed
5. **Kapabilitetskortet tilbydes når det organisatoriske billede (Organisation–org) er klart**

**Beslutningspunkt ved afslutning:** Hvor mange eksterne organisationer konverterede fra individ-besvarelse → organisationsbillede → betalt Kapabilitetskort? Det er din reelle konverteringsrate gennem hele tragten — brug den til at regne baglæns hvor mange henvendelser de sidste kunder kræver.

---

## Fase 4 — Skalering mod 10 (løbende, resten af tidsbudgettet)

**Hvad:** Gentag Fase 3's mekanisme med justeringer baseret på hvor tragten faktisk lækker.

**Hvorfor:** Ved dette punkt har du data nok til at vide om flaskehalsen er **leads** (for få besvarer Positionsanalysen — Individ), **organisatorisk konvertering** (mange individer besvarer, men ingen samler en gruppe under Organisation–individ), eller **produkt/pris** (Organisation–org-billedet er klart, men de siger nej til Kapabilitetskortet).

**Tre forskellige justeringer afhængig af hvad du ser:**

- **Hvis problemet er leads til Individ-niveauet:** Brug Danpo/Scandi-casen som indhold — et kort LinkedIn-opslag der linker direkte til Positionsanalysen
- **Hvis problemet er konvertering fra Individ til Organisation–individ:** Det betyder folk tager testen for egen nysgerrighed, men ingen samler kolleger om det. Overvej om HR/leder skal være indgangen fra start i den eksterne outreach, ikke individet
- **Hvis problemet er Kapabilitetskortets pris/produkt:** Det vigtigste signal — organisationer anerkender gabet, men ikke nok til at betale endnu. Det er et produktspørgsmål: er de seks anvendelser (rekruttering/udvikling/succession & teamdesign/interviewspørgsmål/stillingsopslag/skjulte talenter) tydelige nok i hvad de reelt får?

**Beslutningspunkt:** Ved 10 betalende kunder til Kapabilitetskortet er roadmap'et fuldført. Herfra handler det om pris-optimering, et lettere onboarding-flow, og brug af den aggregerede data i bogens Akt 3.

---

## Hvad der eksplicit IKKE er i dette roadmap

- Markedsføring af bogen som selvstændigt produkt
- Yderligere udvikling af Karrierekompas/Selvdiagnostik udover det der direkte støtter salgsflowet
- Konkurrentanalyse — relevant senere, ikke nu
- Detaljeret prisstrategi for Kapabilitetskortet — sæt en pris, test den, juster baseret på faktiske reaktioner i Fase 1-3
- Capability Stack Analysis og Capability Position Scorecard — to beslægtede, fremtidige produktmuligheder, bevidst udskudt. Se næste afsnit.

---

## Fremtidige muligheder — eksplicit udskudte, ikke aktiveret

Disse to hører ikke til i Fase 0-4. De er navngivet her, så de ikke skal genopfindes senere, og så ressourcerne ikke ved et tilfælde flyder mod dem før det første produkt er bevist i marked.

### Capability Stack Analysis

Spørgsmålet det rejser — "hvor i værdikæden akkumulerer vi, og hvor er vi afhængige af andre aktørers motorer?" — er ikke et spørgsmål om *hvorfor* ACA-mekanismen findes. Det er bogens mekanisme *anvendt* på en specifik virksomhedsbeslutning: værdikædestrategi og leverandørafhængighed. Strukturelt identisk med hvordan Kapabilitetskortet er ACA anvendt på rekruttering — samme familie af produkter, ikke en udvidelse af bogen.

**Hvad det konkret ville være:** En analyse (rapport eller workshop-baseret proces, ikke et selvstændigt instrument som Positionsanalysen) der kortlægger:
- Hvilke led i værdikæden virksomheden selv akkumulerer kapabilitet i — og hvilke den kun er bruger af andres
- Hvor flaskehalsene sidder, som virksomheden er afhængig af, men ikke ejer (jf. bogens Kontinent-kapitel)
- Hvilke afhængigheder er stabile, og hvilke er strukturelt skrøbelige (jf. Fragility Paradox)
- Hvor i kæden et forspring, bygget nu, ville være svært at kopiere om fem år

**Hvorfor det kunne blive særligt værdifuldt:** Det kræver en kombination der er usædvanlig at finde i én person — e-procurement-domænekendskab, direkte ERP/spend-data-erfaring (M3, QlikSense, Acentio), investorlinsen ("køb motorerne, ikke narrativet" anvendt på en kundes egen virksomhed), og hele ACA-frameworket som teoretisk fundament. Det er kombinationen, ikke et enkelt element, der gør produktet svært at kopiere.

**Hvorfor det er udskudt, ikke aktiveret:**
1. Ressourcerne er bundet i Fase 0-4 mod 10 betalende Kapabilitetskort-kunder. Et femte produkt nu spreder fokus før det første er bevist.
2. Det kræver en anden salgskanal — C-suite, strategi eller procurement-direktion, ikke HR. Det er ikke en udvidelse af den eksisterende tragt.
3. Det trækker direkte på Akt 3 (Kontinentet) og Akt 4 (Fragility Paradox), som stadig er under aktiv revision. Det fortjener at bygges efter bogen er færdig, ikke under.

**Aktiveres når:** Bogen er udgivet, de første 10 Kapabilitetskort-kunder er konverteret, og én konkret pilotcase er identificeret — ideelt via Scandi Standard-netværket eller investornetværket, hvor en værdikædeafhængighed kan dokumenteres konkret nok til at blive et bevisstykke.

### Capability Position Scorecard

En separat, men beslægtet mulighed — samme logik som Capability Stack Analysis, men tværgående: i stedet for én virksomheds position i sin egen kæde, placerer scorekortet flere aktører (virksomheder, brancher, stater) relativt til hinanden på samme dimensioner.

**Version 1 — rangordning, ingen ny validering krævet:**
Et scorekort på fem dimensioner, alle allerede etableret i bogens framework — Absorption (PACAP), Integration (RACAP), Koordination, Infrastruktur, Standardmagt. Resultatet er en sætning som *"Lusiaves er her. Scandi er her. Danmark er her. Europa er her."* — en relativ placering, ikke en forudsigelse. Et diagnostisk øjebliksbillede, intet mere.

**Version 2 — kalibreret confidence score, eksplicit databetinget, ikke aktiveret endnu:**
Den mere ambitiøse version: ikke kun "scorer højere end gennemsnittet," men "X procent sandsynlighed for at akkumulere et målbart forspring inden for tre år." Det kræver tre ting der ikke findes endnu — en basisrate (historisk udfald for givne scores), kalibrering (test af om scoren faktisk forudsagde korrekt), og en sagt fejlmargin. Uden de tre er et procenttal en rangordning klædt ud som statistik. Samme validering bogens kapitel 25 kræver af CTI-instrumentet, før det kan kaldes en test.

**Praktisk implikation:** Sælg version 1 nu, hvis og når produktet aktiveres. Omtal version 2 eksplicit som forskningsambition under udvikling — aldrig som en færdig egenskab, før basisrate og kalibrering faktisk er gjort.

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

| Gammelt navn | Nyt navn | Filnavn | Funktion |
|---|---|---|---|
| Skæbnescenariet / Positionsanalysen | **Positionsanalysen — Individ** | `Positionsanalyse_individ.html` | AS-IS, personligt niveau, ingen org-kontekst, gratis/viralt |
| (ny) | **Positionsanalysen — Organisation–individ** | `Positionsanalyse_Org_individ.html` | AS-IS, individniveau med organisations-tag, HR sender internt |
| (ny) | **Positionsanalysen — Organisation–org** | `Positionsanalyse_Org_Org.html` | AS-IS, aggregeret organisationsniveau, HR/leder-indgang |
| Rekrutteringsværktøjet | **Kapabilitetskortet** | `Kapabilitetskortet.html` | TO-BE, betalt, seks anvendelser: rekruttering / udvikling / succession & teamdesign / interviewspørgsmål / stillingsopslag / skjulte talenter |

---

*Roadmap v4 — The Engines Behind / NorthLogicLab*
*Bygget til at blive justeret efter Fase 1's faktiske resultat — ikke en statisk plan.*