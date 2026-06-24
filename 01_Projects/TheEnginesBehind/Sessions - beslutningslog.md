# SESSIONS — The Engines Behind
## Analytisk beslutningslog (kort form)
### Sidst opdateret: 24. juni 2026

---

Dette dokument er bogens analytiske hukommelse — ikke et mødereferat.
Status-først, next-steps-fokuseret. Tidligere historik ligger i tidligere versioner af dette dokument.

---

## LØST KONFLIKT — Akt 4's danske titel (var åben siden 21. juni)

Konflikten beskrevet nedenfor er løst i sessionen 24. juni. Den faktiske, autoritative fil havde 35 forekomster af engelske akt-titler spredt over to forskellige formater — `## Akt X — [engelsk titel]` i kapiteloverskrifter, og `*Akt X — [engelsk titel]*` i fodnoter og case-filers placeringsreferencer. Begge formater er nu rettet konsekvent til de danske titler (Mønstret, Acceleratoren, Strategisk Positionering, Skrøbelighedsparadokset, Motoren Bag Motoren) på tværs af hele manuskriptet, inklusive de seks Akt 1-case-filer. Rettelsen er committet (`86495a7..9650721`).

**Resterende, bevidst urørt:** Akt 4 og Akt 5's titelsider (`# AKT 4 — SKRØBELIGHEDEN` / `## The Fragility Paradox` og samme mønster for Akt 5) har stadig en engelsk undertitel direkte under den danske hovedtitel. Det kan være en bevidst brand-detalje, parallelt med at bogens egen titel ("The Engines Behind") ikke oversættes — ikke rettet ensidigt, afventer en eksplicit beslutning.

Den oprindelige konfliktbeskrivelse, bevaret for historikkens skyld:

> To parallelle sessioner (20. og 21. juni) havde arbejdet på manuskriptet uafhængigt af hinanden, og var ikke afstemt mod samme filversion. Akt 4's danske titel var sat til "Skrøbelighedsparadokset" i én session, mens den faktiske, nyeste fil havde 39 forekomster af den engelske form. Det var uklart hvilken fil var den autoritative nyeste.

---

## Status — hvor projektet står

**Manuskript:** Komplet gennemskrivningsrunde udført på tværs af **alle fem akter (42 kapitler inkl. Interlude)** — sprog- og kildehærdning (session 20. juni). Akt 5's hovedmetafor erstattet (stige → skov/rod), EPOCH operationaliseret, Akt 1's case-numre rettet (session 21. juni). Fem nye teoretiske fundamenter integreret med metaforisk sprog — Coase, Ashby, Hicks, I.J. Good/intelligensexplosion, Piketty/Zucman — samt en kritisk faktarettelse af BCG's 10-20-70-regel og en fuld oprydning af engelske akt-titler (session 24. juni).

**Instrumenter:** Positionsanalysen bekræftet som **tre niveauer plus Kapabilitetskortet**. Kapabilitetskortets seks faner bekræftet fra begge sider af tidligere sessioner.

**Hjemmeside:** Forside og bagside i manifest-stil designet og godkendt — **ikke committet endnu**, afventer at filerne lægges lokalt (status uændret siden 20. juni).

**Roadmap:** v4 — tre instrumentniveauer, seks Kapabilitetskort-anvendelser, Capability Stack Analysis og Capability Position Scorecard som udskudte fremtidsmuligheder.

**Visualisering:** Tre færdige illustrationer for Akt 4's Fragility Paradox (Robust/Fragil/Antifragil) bygget på Talebs skelnen, med træ/rod-billedsprog konsistent med bogens hovedmetafor — leveret som separate billedfiler, ikke endnu indsat i selve manuskriptteksten.

**Git:** Terminologi- og kildehærdning fra 20. juni committet (`4ba62c9..23babcc`). Akt 1-rækkefølge, skov-metafor, EPOCH, roadmap v4 fra 21. juni committet (`23babcc..03f840f`, opfølgning `03f840f..5654f2e`). Teoretisk styrkelse, BCG-faktarettelse og akt-titel-oprydning fra 24. juni committet og pushet (`86495a7..9650721`).

---

## 2026-06-24 — Teoretisk styrkelse, BCG-faktarettelse, akt-titel-oprydning, Taleb-visualisering

**Det vi løste:**

Fem nye teoretiske fundamenter undersøgt, kritisk vurderet, og integreret med metaforisk sprog i stedet for tør teorihenvisning:

- **Coases teori om virksomhedens grænser (1937)** — hvorfor virksomheder vokser ved at internalisere transaktioner der er dyrere at forhandle på markedet. Integreret i Ford-casen (husstand/restaurant-analogi: lave maden selv vs. bestille take-away) og som kort krydsreference i Organisationen-kapitlets "Tre organisationer, samme Oversætter".
- **Ashby's lov om nødvendig variation (1956)** — kun variation kan absorbere variation. Integreret i Effektivitetens pris-kapitlet med skib/storm-analogi, og gør "slack er en dæmper"-argumentet til en formel lov i stedet for kun en metafor.
- **Hicks' induced innovation-hypotese (1932)** — relative faktorpriser retter teknologi mod at erstatte den dyreste faktor. Brugt i Akt 5's double-compounding-hypotese, med en eksplicit, selvkritisk korrektion: den oprindelige anvendelse var for firkantet (ignorerede substitutionselasticitet — høj pris fører kun til erstatning hvor erstatning faktisk er teknisk mulig, ellers fører den til investering i bevarelse).
- **I.J. Good (1965), Amodei, Kaplan, Bengio** — intelligensexplosion tilføjet som sjette, åben grænsebetingelse i kapitel 25. Kurzweil bevidst afvist som kilde (manglende metodologisk disciplin, historik af ikke-verificerede datoer) efter direkte undersøgelse af kritikken af hans seneste bog.
- **Piketty (r > g), Zucman (skattely), World Inequality Report 2026** — tilføjet til Rockefeller-casen med konkret, målt accelerationsrate (8% årligt hos milliardærer mod under 4% siden 1990'erne). Syvende grænsebetingelse tilføjet i kapitel 25: vi kan kun måle koncentration der ikke er gjort usynlig. Pikettys kritiker (Góes/IMF) undersøgt grundigt efter direkte spørgsmål om kritikkens berettigelse — fundet at være en reel, teknisk metodeindvending (forkert proxy for kapitalafkast), ikke kun politisk motiveret, men at Zucmans uafhængige skattely-forskning samtidig styrker Pikettys side af striden betydeligt.

**Kritisk faktarettelse, fundet ved sammenligning af to parallelle redaktionsspor:** Organisationen-kapitlet (3.7) i den autoritative arbejdsfil havde stadig den **fejlciterede** udgave af BCG's "70-20-10-regel" stående — en påstået fordeling af virksomheder i tre adoptionslag (70% deployer, 20% integrerer, 10% redesigner). Et uploadet, parallelt redigeret eksemplar af samme kapitel havde den **korrekte** version (verificeret direkte mod BCG.com): en fordeling af *værdi* i en AI-implementering (10% algoritme, 20% teknologi/data, 70% proces/mennesker). De to spor blev sammenlagt — korrekt BCG-fakta fra det ene spor, nyere Coase-tilføjelse og WEF/Cedefop/Simvia-syntese fra det andet, ingen af delene tabt.

**Akt-titel-oprydning, to lag:** Et tidligere forsøg på at rette engelske akt-titler havde kun fanget `## Akt X — [titel]`-formatet i kapiteloverskrifter. En bredere gennemgang fandt 35 yderligere forekomster i `*Akt X — [titel]*`-fodnotestilen (kursiv) og i de seks Akt 1-case-filers `*Placering: Akt X — [titel]*`-linjer. Alle rettet konsekvent. Organisationen-kapitlets nummerering rettet fra "### 2." til "### 3.7 —" efter direkte instruktion.

**Taleb-baseret visualisering, Akt 4 Fragility Paradox:** Iterativt arbejde gennem tre forsøg. Første (fire separate paneler, hver egen akse) afvist: ingen synlig sammenhæng. Andet (ét samlet diagram, normaliseret akse, alle cases lagt på arketype-skygger) afvist: for meget information i ét billede. Tredje, endelige tilgang: tre separate, fokuserede billeder (Robust/Fragil/Antifragil), hver med kurve + træ-illustrationer (krone og synlige rødder under jorden) i stedet for kun abstrakte kurver — konsistent med bogens skov/rod-hovedmetafor. Central pointe indbygget visuelt i Fragil-billedet: det første træ er mærket "så sundt ud — men roden var svag", fordi fragilitet per definition er usynlig før chokket. Antifragil-billedet bærer en eksplicit ærlighedsklausul: ingen af bogens egne cases dokumenterer denne form i Talebs strenge forstand.

**57 stående `-e`-formateringsrester** fundet og fjernet fra hele `book_updated.md` — en gammel artefakt fra tidligere shell-ekstraktioner.

**Beslutninger der ikke kan omgøres:**

Alle akt-titler er danske i både kapiteloverskrifter og fodnoter, konsekvent: Mønstret, Acceleratoren, Strategisk Positionering, Skrøbelighedsparadokset, Motoren Bag Motoren.

Coase, Ashby, Hicks, I.J. Good og Piketty/Zucman behandles alle med samme forsigtighed: mekanisme som forklaringskraft, eksplicit markeret hvor de er omstridt eller ikke direkte udviklet til AI-kontekst.

BCG's 10-20-70 er en fordeling af værdi i en AI-implementering, ikke en fordeling af virksomheder efter modenhed. Denne distinktion må ikke driftes tilbage til den fejlciterede version.

**Forkastede retninger:**

To af tre visualiseringsforsøg for Talebs robust/fragil/antifragil-skelnen — begge forkastet for at presse for meget information ind i ét billede, ikke for faktuel fejl.

En sammensat, vægtet "Fragility Score" (fem dimensioner: koncentration, redundans, koblingsgrad, adaptiv kapacitet, social sammenhængskraft) — forkastet efter kritisk modspil: en vægtet sammensætning af usammenlignelige enheder er pseudo-præcis, samme svaghedstype som allerede identificeret i andre kilders metodefejl.

**Output:**

`THE_ENGINES_BEHIND_KOMPLET.md` (fuld bog, opdateret og oprenset)
`akt3-kap7-organisationen.md` (rettet nummerering + BCG-fakta)
`akt4-kap8-effektivitetens-pris.md`, `akt4-kap11-systemskaberen-flaskehals.md` (akt-titel-rettelse)
`A1_robust.png`, `A2_fragil.png`, `A3_antifragil.png` (Taleb-træ-illustrationer)
`commit-session.ps1`

**Åbne spørgsmål:**

Akt 4 og Akt 5's titelsider har stadig en engelsk undertitel under den danske hovedtitel ("The Fragility Paradox", "The Engine Behind the Engine") — ikke rettet, afventer eksplicit beslutning om det er en bevidst brand-detalje.

Et fjerde Taleb-visualiseringsbillede (stats-/kontinentniveau, samme træ-skabelon) er ikke bygget.

Integrationstekst der binder de tre færdige Taleb-billeder ind i selve Akt 4-manuskriptet er ikke skrevet — billederne eksisterer som separate filer, ikke som indsat bogindhold.

"Tacit knowledge" i Akt 4 kapitel 10 — status ikke reverificeret i denne session, tidligere flaget som ikke fuldt rettet.

**Næste træk:**

Afklar om Akt 4/5's engelske undertitler skal blive eller rettes. Byg det fjerde Taleb-billede (kontinenter) hvis ønsket. Skriv integrationstekst for Taleb-billederne ind i Akt 4. Fortsæt fintuning af rekrutteringsværktøjerne (uændret fra 21. juni's prioritet).

---

## 2026-06-21 — Skov-metafor i Akt 5, EPOCH-operationalisering, DeepSeek-reframing, roadmap v4, case-rækkefølge

**Det vi løste:**

Stigemetaforen i Akt 5 erstattet med skov/rod — "tyve træer, et eller to dominerer ved år 30" gør koncentration synlig som en hel population, ikke kun konkurrence mellem to. Mycorrhiza-netværket tilføjet som billede på relationer/koordinering/institutioner, der binder individ/organisation/stat/kontinent til "samme figur, fire skalaer".

"Tre baner" tilføjet som Akt 5's afsluttende scenarie-syntese — flad verden / stor ulighed / skrøbelighed eksploderer. Bevidst kaldt "baner", ikke "Verden A/B/C", for at undgå navnekollision med kapitel 9's allerede etablerede scenarier på individniveau.

Double-compounding-hypotesen (konverteringsraten stiger selv, ikke kun grundlaget den beregnes af) udvidet med DeepSeek R1 som konkret empirisk eksempel. Samme reframing i kapitel 25, Grænse 1: DeepSeek vendt fra defensiv ("stærkeste udfordring mod ACA") til offensiv (skarpeste bekræftelse — gratis adgang for alle kan pr. definition ikke være differentieringsfaktoren). Videnskabelig forsigtighed bevaret begge steder.

Grænse 5 tilføjet til kapitel 25 — ACA's stumhed om individets handlekraft når konverteringsmekanismen er strukturelt lukket. Eksplicit markeret som en anden type grænse end de første fire (konstaterbar, ikke testbar med data). Tre forankrede, ikke-trøstende fragmenter af svar givet, ingen falsk trøst.

Falsifikationsbetingelser i kapitel 25 skærpet med konkret operationel tærskel — BCG's 1,7x/3,6x øjebliksbillede testet som et langsgående krav over fem til ti år, ikke kun korrelation.

"Industrial Absorption Systems"-rammen skrevet ind i Akt 3's åbning. Kinas klimateknologi tilføjet til Staten-kapitlets demokrati/autoritær-dilemma — eksplicit skilt fra TSMC/ASML's markedsdrevne akkumulering.

EPOCH (Loaiza & Rigobon, MIT Sloan) operationaliseret fra egenskaber til adfærdsspørgsmål i bogens eget sprog: Systemforståelse, Situationsforståelse, Beslutningskapacitet, Rekombinationskapacitet, Koordinationskapacitet. Eksempler bygget i sales/økonomi i stedet for procurement. Skrevet ind i rekrutteringskapitlet og Akt 5 kapitel 3. Valideringsdisclaimer tilføjet.

Lusiaves/Scandi-interludet fået konkret indhold: 2027 EBIT-mål og kvartalsdata, korrigeret fra blandet kvartalssammenligning til år-over-år efter at Q3's sæsonalitet blev flaget. 2032-strategien eksplicit udeladt — afventer officiel offentliggørelse.

Akt 1's case-rækkefølge rettet til kanonisk EIC(1)/Rockefeller(2)/Ford(3)/Toyota(4)/Intel(5)/Maersk(6) — gennemført både i den samlede bogfil og i de seks individuelle case-filer (overskrift, fodnote-titel og placeringsreference rettet konsekvent i alle tre lag, i alle seks filer).

Akt 4 kapitel 6's overskrift ændret fra "Standard Oil og den pyrrhussejr" til "Standard Oil og sejren der blev sin egen undergang" — selvforklarende uden at kræve forhåndskendskab til Pyrrhus-referencen.

"Kognitiv stratifikation" (kapitel 9) fået en kort forklaring af selve ordet — afviste en foreslået neuropsykologisk analogi (forkert felt, ville modsige kapitlets pointe om at stratifikationen er strukturel, ikke individuel), valgte skoven, genbrugt fra Akt 5 for konsistens.

Roadmap rettet fra to til tre instrumentniveauer for at matche faktiske filnavne — fandt at roadmap'ens Fase 1 fejlagtigt brugte det tag-løse Individ-instrument til Danpo-pilotens data, hvilket ville have gjort aggregering umulig. Rettet til Organisation–individ. Kapabilitetskortet rettet fra fire til seks anvendelser. Capability Stack Analysis og Capability Position Scorecard tilføjet som eksplicit udskudte, fremtidige produktmuligheder.

Generel terminologi-oprydning fortsat: "replication barriers" → "barriere mod kopiering", "deployer" → "udruller", "Process Keeper" → "Systemfølgeren" konsekvent i kapitel 11 og 12.

**Beslutninger der ikke kan omgøres:**

Skoven/roden er nu bogens eneste hovedmetafor for akkumulering over tid — stigen er fuldt udfaset.

"Baner", ikke "Verden A/B/C", er navnet på Akt 5's afsluttende scenarie-syntese. Verden A/B/C forbliver låst til kapitel 9's individniveau.

DeepSeek og lignende AI-effektivitetsspring behandles som bekræftelse af ACA, ikke som trussel mod den.

Statsdrevet og markedsdrevet akkumulering er to forskellige veje til samme udfald, og skal altid eksplicit skilles fra hinanden når begge eksemplificeres i samme afsnit.

EPOCH-kategorierne hedder Systemforståelse/Situationsforståelse/Beslutningskapacitet/Rekombinationskapacitet/Koordinationskapacitet i bogens sprog — MIT's originale akronym krediteres som kilde, bruges ikke som bogens egne etiketter.

**Forkastede retninger:**

Neuropsykologisk hjernehierarki-model som forklaring på "kognitiv stratifikation" — forkastet, forkert felt.

Geologisk lag-analogi til samme begreb — overvejet, forkastet for konsistens med skoven.

"Capability Early Warning System" som produktnavn — forkastet, for kategorisk et løfte. Erstattet af "Capability Position Scorecard" med eksplicit to-trins struktur.

**Output:**

`THE_ENGINES_BEHIND_KOMPLET.md`, `THE_ENGINES_BEHIND.pdf`
`akt3-aabning.md`, `akt3-kap2-organisationen.md`, `akt3-kap3-staten.md`, `akt3-kap14b-rekruttering.md`
`akt4-kap4-koordinationskollaps.md`, `akt4-kap6-legitimitetserosion.md`, `akt4-kap11-systemskaberen-flaskehals.md`
`akt5-kap3-syntese-slutposition.md`, `akt5-kap25-aca-forklaringsmotor.md`
`interlude-lusiaves-scandi.md`
`1.1 EIC.md` til `1.6 Maersk.md` (case-filer, rettet rækkefølge)
`Roadmap_v4.md`
`alle_ser_kronen.png`
`commit-simple.ps1`

**Åbne spørgsmål:**

Akt 4's danske akt-titel ("Skrøbelighedsparadokset" vs. "The Fragility Paradox") — se ÅBEN KONFLIKT øverst i dette dokument. Skal afklares før næste commit rører Akt 4.

"Tacit knowledge" stadig ubehandlet engelsk i kapitel 10, mens kapitel 9 og resten af bogen bruger "tavs viden".

Capability Stack Analysis og Capability Position Scorecard er navngivet og placeret i roadmap'en, men ikke designet som produkt.

Positionsanalysen er ikke koblet til "Tre baner" — diskuteret, ikke bygget.

**Næste træk:**

Fintune rekrutteringsværktøjerne — Kapabilitetskortet og de tre Positionsanalyse-niveauer. Sandsynligt fokus: bekræfte Organisation–individ → Organisation–org-aggregeringen virker med rigtige data, og at de seks Kapabilitetskort-anvendelser er konsistente med EPOCH-operationaliseringen.

---

## 2026-06-20 — Sprog- og terminologioprydning (hele bogen)

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

**Akt-titler — alle fem oversat og gennemført konsekvent (se ÅBEN KONFLIKT for Akt 4-status):**

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

## Instrumenter — B2C/B2B-arkitektur (bekræftet fra to uafhængige sessioner)

**Strategisk beslutning:** Positionsanalysen er splittet i tre niveauer plus Kapabilitetskortet, med klart adskilte formål:

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
  (rekruttering, udvikling, succession, teamdesign, interview, opslag,
  skjulte talenter — seks anvendelser i alt) er her.
```

**Nøglebeslutning om distributionsrækkefølge:** Kæden er **Problem → P-Organisation → Kapabilitetskort**, ikke P-Individ → P-Organisation → Kapabilitetskort. HR køber ikke fordi en medarbejder delte en personlighedstest — de køber fordi de allerede har et navngivet problem. P-Individ er en parallel, selvstændig brand-awareness-motor, ikke trin 1 i en B2B-salgstragt.

**Distributionsprioritet (kort til langt sigt):** 1) Direkte relationer (Scandi, netværk, møder) → 2) Interne champions (en HR-medarbejder finder værktøjet og overbeviser sin egen organisation) → 3) Organisk inbound (SEO, content) — bevidst nedprioriteret til produktet er bevist i lukkede relationer.

**Kapabilitetskortet — fejl rettet, anvendelser navngivet korrekt:**
1. Sekvens-guidens fortælling synkroniseret 1-til-1 med de faktiske seks faner (①ACA-analyse → ②Udvikling → ③Succession & Teamdesign → ④Interviewspørgsmål → ⑤Stillingsopslag → ⑥Skjulte talenter). Roadmap'en havde tidligere kun navngivet fire af de seks — rettet.
2. Interviewspørgsmålene i Stillingsopslag-fanen var identiske og hardkodede for alle fem arketyper. Hver arketype har nu sit eget, relevante sæt af tre spørgsmål.
3. Aktiv fane-tilstand i navigationen gjort markant tydeligere.
4. Roadmap'ens Fase 1 brugte fejlagtigt det tag-løse P-Individ-instrument til pilotdata, som derfor ikke kunne have været aggregeret — rettet til P-Org-individ.

**Simvia/PPWR-kilden** er bygget ind to steder med forskellig funktion: 3.7 (empirisk bevis i bogteksten) og `The_connection`-strategidokumentet (kommercielt åbningsargument med hård deadline, målt tal og total markedsudelukkelse som sanktion).

---

## Hjemmeside — forside og bagside

To gamle HTML-artifacts (`Frontpage.html`, `Backpage.html`) viste sig at være ubrugelige browser-snapshots af chatgrænsefladen, ikke den faktiske kode — samme problem som tidligere fundet med "Priksekvensen" og "Translation_Barrier"-filerne. **Ikke genfindelige.**

Begge sider er i stedet genbygget fra grunden, **godkendt iterativt mod skærmbilleder** af det faktiske, ønskede design (centreret poesi-lag-stil, sort baggrund, amber accenter):

- **Forside:** "Adgang distribueres. Fordel koncentreres." + "Hvorfor?" + slutmanifest.
- **Bagside:** Tre historiske strofer (Rockefeller/jernbanen, Toyota/fabriksgulvet, TSMC/uerstattelig) → "Adgang bliver billigere / Kapabilitet bliver vigtigere / Forskellen vokser" → thesis: *"Dette er ikke en bog om AI. Det er en bog om, hvorfor nogle aktører akkumulerer — mens andre starter forfra."*

**Status:** Filerne er klar, men er **ikke lagt ind i det lokale repo eller committet endnu** — afventer at Jon henter dem til `C:\Dev\NorthLogicLab` og kører en separat commit.

**Bemærkning til senere:** Hjemmesidens marketing-tekst bruger nu tre lidt forskellige formuleringer af samme grundmekanisme på tværs af forskellige flader — "adgang/konvertering" (bogens narrative tekst), "adgang/kapabilitet" (bagside), "adgang/fordel" (forside). Ikke nødvendigvis et problem (marketing-tekst kan tillade sig mere variation end bogens prosa), men værd at tage stilling til bevidst, hvis det skal strammes til ét fast ordpar.

---

## Næste skridt — prioriteret

```
1. Afklar om Akt 4/5's engelske undertitler ("The Fragility Paradox",
   "The Engine Behind the Engine") skal blive eller rettes til dansk
2. Hjemmeside: hent forside/bagside-filer lokalt, læg i repo, commit separat
3. Byg det fjerde Taleb-visualiseringsbillede (stats-/kontinentniveau,
   samme træ-skabelon som Robust/Fragil/Antifragil)
4. Skriv integrationstekst der binder de tre færdige Taleb-billeder
   ind i selve Akt 4-manuskriptet — de eksisterer i dag kun som separate
   billedfiler, ikke som indsat bogindhold
5. Fintune rekrutteringsværktøjerne — bekræft P-Org-individ → P-Org-Org-
   aggregeringen virker med rigtige data, verificer de seks Kapabilitetskort-
   anvendelser er konsistente med EPOCH-operationaliseringen
6. Resterende engelske termer: "tacit knowledge" i Akt 4 kapitel 10 — sidst
   flaget (21. juni) som endnu ikke rettet til "tavs viden", selvom kapitel 9
   og resten af bogen allerede er det. Ikke reverificeret i denne session.
7. Indledningen: bekræftet i god stand, ingen ændring nødvendig
8. Fitness-analogien fra 3.3: overveje om den skal genbruges som UI-tekst
   i Positionsanalyse-instrumenterne (tidligere besluttet, ikke udført endnu)
9. Kritisk manuskriptgennemlæsning (Akt 1 primært) — uændret fra tidligere
   sessioner, stadig åbent: falsifikation per case, source hardening,
   "Hvad lederen ser"-bokse, gentagelsesreduktion, "hun" som narrativ tråd
10. SIMVIA/regulatorisk kæde — PPWR er nu kildehærdet og indsat.
    ESPR/AI Act/CSRD/EUDR-resten af kæden fra The_connection er stadig
    ikke selvstændigt verificeret med samme grundighed
11. Capability Stack Analysis og Capability Position Scorecard (roadmap v4)
    er navngivet, ikke designet — ingen konkret produktspecifikation endnu
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
- Skoven/roden er bogens eneste hovedmetafor for akkumulering over tid (21. juni — erstatter en tidligere stigemetafor)
- "Baner", ikke "Verden A/B/C", er navnet på Akt 5's scenarie-syntese; Verden A/B/C forbliver låst til kapitel 9's individniveau
- Akt 1's case-rækkefølge er EIC(1)/Rockefeller(2)/Ford(3)/Toyota(4)/Intel(5)/Maersk(6) — gennemført i både samlet bogfil og de seks individuelle case-filer
- Alle akt-titler er danske, konsekvent, i både kapiteloverskrifter og fodnoter — Mønstret, Acceleratoren, Strategisk Positionering, Skrøbelighedsparadokset, Motoren Bag Motoren (24. juni — løste en tidligere åben konflikt mellem to redaktionsspor)
- BCG's 10-20-70 er en fordeling af værdi i en AI-implementering (10% algoritme, 20% teknologi/data, 70% proces/mennesker) — ikke en fordeling af virksomheder efter modenhed. Den fejlciterede version må ikke gentages
- Organisationen-kapitlet hedder 3.7, ikke "2." — Akt 3's bredere nummereringsinkonsistens (blandede stilarter: Kapitel 13/14a/14b, 1c, 3.7, 4, 5) forbliver et åbent, ikke-besluttet spørgsmål

---

*SESSIONS.md — The Engines Behind*
*Opdateres ved afslutning af hver session.*