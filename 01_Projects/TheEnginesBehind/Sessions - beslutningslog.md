# SESSIONS — The Engines Behind
## Analytisk beslutningslog (kort form)
### Sidst opdateret: 20. juni 2026

---

Dette dokument er bogens analytiske hukommelse — ikke et mødereferat.
Status-først, next-steps-fokuseret. Tidligere historik ligger i tidligere versioner af dette dokument.

---

## Status — hvor projektet står

**Manuskript:** Komplet gennemskrivningsrunde udført på tværs af **alle fem akter (42 kapitler inkl. Interlude)**. Dette var ikke nyt indhold — det var en samlet sprog- og kildehærdningsrunde, der gør hele manuskriptet konsistent for første gang siden de individuelle akter blev skrevet i separate sessioner.

**Instrumenter:** Positionsanalysen er omstruktureret fra to til **fire værktøjer** med en klar B2C/B2B-arkitektur. Kapabilitetskortet er rettet for to konkrete fejl (tab-nummerering, arketype-specifikke interviewspørgsmål).

**Hjemmeside:** Forside og bagside i manifest-stil er designet, godkendt mod skærmbilleder af det oprindelige (ikke-genfindelige) design, og klar til at lægges ind i repoet — **ikke committet endnu**, afventer at filerne lægges lokalt.

**Git:** Hele terminologi- og kildehærdningsrunden er committet og pushet (`4ba62c9..23babcc`).

---

## Det store arbejde — sprog- og terminologioprydning (hele bogen)

**Baggrund:** PACAP/RACAP og en række engelske akademiske termer (Institutional Fusion, Architectural Embedding, Translation Barrier, Process Keeper, m.fl.) var spredt ud gennem alle fem akter fra tidligere skriveperioder. Et gammelt Begrebsregister (2026-05-21) havde planlagt en delvis oprydning, men var aldrig fuldt udført, og var i flere tilfælde overhalet af bedre beslutninger taget direkte i manuskriptet.

**Gennemført, akt for akt:**

- **Akt 1 — Mønstret** (7 kapitler): Engelske krydsningsarketyper oversat — Institutional Fusion → Institutionel fusion, Architectural Embedding → Strukturel indlejring, Strategic Reconfiguration → Strategisk rekonfiguration, Network Coordination → Netværkskoordination, Coordination Insight → Koordinationsindsigt, Organizational Memory → Organisatorisk hukommelse. Desuden rettet: switching costs → skifteomkostninger, "The Six Crossings" → "De seks krydsninger" (filnavn omdøbt), RACAP → konvertering. Case-numre i footer rettet til at matche filnavnenes 1.1–1.7-nummerering (var tidligere inkonsistente — Intel sagde "Case 6", Toyota sagde "Case 4").

- **Akt 2 — Acceleratoren** (7 kapitler): Allerede stort set rene fra en tidligere v2.0-revision. Kun akt-titlen og én RACAP-sætning (i "Ejer du accelerationen") krævede rettelse.

- **Interlude — Motoren i Realtid** (Scandi/Lusiaves-casen): Kun titlen var engelsk. Resten af kapitlet brugte allerede korrekt dansk terminologi.

- **Akt 3 — Strategisk Positionering** (9 kapitler, 3.1–3.9): Det tungeste arbejde. Ud over terminologi blev der fundet og rettet en **faktuel fejl**: BCG's "70-20-10-regel" var fejlciteret som en fordeling af virksomheder (70% deployer, 20% integrerer, 10% redesigner) — den faktiske BCG-regel er en fordeling af *værdi* i en AI-implementering (10% algoritme, 20% teknologi, 70% proces/mennesker), verificeret direkte mod BCG.com. Rettelsen styrker kapitlets pointe i stedet for at svække den. Desuden: ASML-komponentpåstanden ("mere end 10% amerikansk teknologi") var sat for lavt — korrekt og stærkere version er at ASML selv kun producerer ca. 15% af komponenterne, resten kommer fra et globalt netværk inkl. kritisk amerikansk laserteknologi (Cymer). Simvia/PPWR-eksemplet (35% readiness, august 2026-deadline) tilføjet i 3.7 som konkret bevis for regulatorisk Conversion Gap.

- **Akt 4 — Skrøbelighedsparadokset** (11 kapitler): Tungt PACAP/RACAP- og engelsk-indhold. Vigtigst: **"Process Keeper" var en uoversat arketype** i kapitel 4.11 — rettet til **Systemfølgeren**, den allerede etablerede danske arketype fra Akt 2/3. Det er ikke kun en oversættelse — det styrker kapitlets pointe, fordi læseren nu genkender profilen i stedet for at møde et nyt navn for noget de allerede kender. Desuden rettet: tacit knowledge → tavs viden, switching costs → skifteomkostninger, replication barrier → replikeringsbarrieren.

- **Akt 5 — Motoren Bag Motoren** (6 kapitler): Samme mønster som Akt 4 — Process Keeper, PACAP/RACAP, Fragility Paradox oversat konsekvent. Fundet og rettet to UI-rest-linjer i bunden af 5.4 (kopieringsfejl fra en tidligere filoverførsel — samme mønster fandtes også i 4.4 i en tidligere runde). **5.6 ("Køb motorerne. Ikke narrativet.") er bevidst tom udover de to ord — ikke en fejl, det er kapitlets pointe udført præcist som tidligere besluttet.**

**Gennemgående regel etableret (ny beslutning, tilsidesætter maj-planen):**
PACAP/RACAP er fjernet fra al narrativ tekst og eksisterer nu **kun formelt ét sted i hele bogen** — kapitel 3.3 — som teoretisk ankring til Zahra & George (2002). Resten af bogen bruger **adgang/konvertering**. En **fitness-analogi** ("Adgang er abonnementet. Konvertering er at rent faktisk træne.") er indsat direkte efter denne introduktion som bro mellem det akademiske sprog og bogens eget sprog.

**Akt-titler — alle fem oversat og gennemført konsekvent:**

| Akt | Dansk titel |
|---|---|
| 1 | Mønstret |
| 2 | Acceleratoren |
| 3 | Strategisk Positionering |
| 4 | Skrøbelighedsparadokset |
| 5 | Motoren Bag Motoren |

*Bogens egen titel ("The Engines Behind") og brand-eyebrowet på hjemmesiden er bevidst ikke oversat — det er navnet, ikke en akt-betegnelse.*

**Begrebsregister opdateret til v2** — dokumenterer nu de faktiske, gennemførte beslutninger (adgang/konvertering, Oversættelsesbarrieren og Hastighedsasymmetri som faste danske begreber, Data Translator/Capability Architect sammenlagt til Oversætteren/Systemskaberen) i stedet for den oprindelige, delvist overhalede maj-plan.

**Gammel metodefil skrottet** — en engelsk "Theory and Method Instruction"-fil blev identificeret som en forældet, men ikke modsagt, tidligere version af den nuværende Core Project Instruction. Ingen indholdsmæssig konflikt — ren duplikering. Slettet og committet (`deleted: Methods`).

---

## Instrumenter — ny B2C/B2B-arkitektur

**Strategisk beslutning:** Positionsanalysen er splittet i fire værktøjer med klart adskilte formål, efter en grundig afklaring af go-to-market-logikken:

```
P-Individ (B2C)         → Positionsanalyse_individ.html
  Ren teaser. Ingen org-tag. Bekymring → Position → Refleksion → Deling.
  Drivkraft: personlig identifikation, ikke organisatorisk salg.

P-Org-individ (B2B)     → Positionsanalyse_Org_individ.html
  Samme spørgsmål som P-Individ, men med org-tag og storage-skrivning.
  IKKE et selvstændigt produkt — kun datainput til P-Organisation.
  Distribueres direkte af HR/ledelse internt.

P-Org-Org (B2B)         → Positionsanalyse_Org_Org.html
  Hovedindgangen. Hero omskrevet fra mekanik til navngivet HR-problem
  ("Hvilke kapabiliteter mangler I?"). Arketype-fordeling nu låst til
  hierarkisk rækkefølge (Systemfølgeren → Systemskaberen), ikke sorteret
  efter antal besvarelser.

Kapabilitetskortet (B2B) → Kapabilitetskortet.html
  Handlingslaget. Diagnose er gratis i de tre ovenstående — handling
  (rekruttering, udvikling, succession, teamdesign) er her.
```

**Nøglebeslutning om distributionsrækkefølge:** Kæden er **Problem → P-Organisation → Kapabilitetskort**, ikke P-Individ → P-Organisation → Kapabilitetskort. HR køber ikke fordi en medarbejder delte en personlighedstest — de køber fordi de allerede har et navngivet problem. P-Individ er en parallel, selvstændig brand-awareness-motor, ikke trin 1 i en B2B-salgstragt.

**Distributionsprioritet (kort til langt sigt):** 1) Direkte relationer (Scandi, netværk, møder) → 2) Interne champions (en HR-medarbejder finder værktøjet og overbeviser sin egen organisation) → 3) Organisk inbound (SEO, content) — bevidst nedprioriteret til produktet er bevist i lukkede relationer.

**Kapabilitetskortet — to konkrete fejl rettet:**
1. Sekvens-guidens fire-trins-fortælling matchede ikke de faktiske seks faner i UI'en — nu synkroniseret 1-til-1 (①ACA-analyse → ②Udvikling → ③Succession & Teamdesign → ④Interviewspørgsmål → ⑤Stillingsopslag → ⑥Skjulte talenter).
2. Interviewspørgsmålene i Stillingsopslag-fanen var identiske og hardkodede for alle fem arketyper — herunder spørgsmål skrevet til Oversætteren/Systemskaberen-profilen, der blev stillet blindt til Fageksperten-kandidater. Hver arketype har nu sit eget, relevante sæt af tre spørgsmål.
3. Aktiv fane-tilstand i navigationen var for diskret (kun 2px understregning) — nu markant tydeligere med fuld baggrundsfarve.

**Simvia/PPWR-kilden** er bygget ind to steder med forskellig funktion: 3.7 (empirisk bevis i bogteksten) og `The_connection`-strategidokumentet (kommercielt åbningsargument med hård deadline, målt tal og total markedsudelukkelse som sanktion).

---

## Hjemmeside — forside og bagside

To gamle HTML-artifacts (`Frontpage.html`, `Backpage.html`) viste sig at være ubrugelige browser-snapshots af chatgrænsefladen, ikke den faktiske kode — samme problem som tidligere fundet med "Priksekvensen" og "Translation_Barrier"-filerne. **Ikke genfindelige.**

Begge sider er i stedet genbygget fra grunden, **godkendt iterativt mod skærmbilleder** af det faktiske, ønskede design (centreret poesi-lag-stil, sort baggrund, amber accenter):

- **Forside:** "Adgang distribueres. Fordel koncentreres." + "Hvorfor?" + slutmanifest.
- **Bagside:** Tre historiske strofer (Rockefeller/jernbanen, Toyota/fabriksgulvet, TSMC/uerstattelig) → "Adgang bliver billigere / Kapabilitet bliver vigtigere / Forskellen vokser" → thesis: *"Dette er ikke en bog om AI. Det er en bog om, hvorfor nogle aktører akkumulerer — mens andre starter forfra."*

**Status:** Filerne er klar i Claude outputs, men er **ikke lagt ind i det lokale repo eller committet endnu** — afventer at Jon henter dem til `C:\Dev\NorthLogicLab` og kører en separat commit.

**Bemærkning til senere:** Hjemmesidens marketing-tekst bruger nu tre lidt forskellige formuleringer af samme grundmekanisme på tværs af forskellige flader — "adgang/konvertering" (bogens narrative tekst), "adgang/kapabilitet" (bagside), "adgang/fordel" (forside). Ikke nødvendigvis et problem (marketing-tekst kan tillade sig mere variation end bogens prosa), men værd at tage stilling til bevidst, hvis det skal strammes til ét fast ordpar.

---

## Næste skridt — prioriteret

```
1. Hjemmeside: hent forside/bagside-filer lokalt, læg i repo, commit separat
2. Akt 1 til 4's "Hvad lederen ser"-bokse og øvrige Akt 2-3 kapitler:
   gennemgå for evt. resterende, ikke-fundne engelske termer
   (denne runde fangede det meste, men er ikke 100% udtømmende testet)
3. Indledningen: bekræftet i god stand, ingen ændring nødvendig
4. Fitness-analogien fra 3.3: overveje om den skal genbruges som UI-tekst
   i Positionsanalyse-instrumenterne (tidligere besluttet, ikke udført endnu)
5. Kritisk manuskriptgennemlæsning (Akt 1 primært) — uændret fra sidste
   session, stadig åbent: falsifikation per case, source hardening,
   "Hvad lederen ser"-bokse, gentagelsesreduktion, "hun" som narrativ tråd
6. SIMVIA/regulatorisk kæde — PPWR er nu kildehærdet og indsat.
   ESPR/AI Act/CSRD/EUDR-resten af kæden fra The_connection er stadig
   ikke selvstændigt verificeret med samme grundighed
```

---

## Beslutninger der ikke kan omgøres (opdateret)

- "Køb motorerne. Ikke narrativet." — slutter Kapitel 5.6, ingen forklaring, ingenting efter
- ACA er konvertering, ikke adgang — må ikke drifte tilbage til adgangsframing
- PACAP/RACAP lever kun formelt i 3.3 — al øvrig tekst bruger adgang/konvertering
- Lusiaves/Scandi Standard: strukturanalyse, ingen intentionsattribuering
- CTI-instrumentet: eksplicit markeret som teoretisk afledt, ikke empirisk valideret
- Fem arketyper låst: Systemfølgeren / Fageksperten / Procesbyggeren / Oversætteren / Systemskaberen — "Oversætteren" betegner nu både individets karriereprofil og fjerde arketype-trin; samme ting set fra to vinkler, ikke to begreber
- Manifest-tone, ikke akademisk — korte deklarative sætninger
- P-Individ forbliver ren B2C uden organisatorisk salgslogik — B2B-broen ligger i P-Organisation, ikke i P-Individ

---

*SESSIONS.md — The Engines Behind*
*Opdateres ved afslutning af hver session.*