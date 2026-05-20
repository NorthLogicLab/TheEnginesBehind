# /critique — Teknisk gæld og åbne spørgsmål

## Teknisk gæld

### HTML arkitektur — Del 1
**Status:** Åben
**Prioritet:** Lav — adresseres efter indholdsgodkendelse

Nuværende output er én monolitisk HTML-fil (~1200 linjer).
Skal splittes når indhold er godkendt:

del1/
  index.html        ← struktur og indhold
  styles.css        ← al styling
  charts.js         ← Chart.js logik
  data/
    capex.json
    nordic-matrix.json
    smile-curve.json

shared/
  base.css          ← fælles typografi og CSS-variabler
  personas.css      ← persona-blokke på tværs af dele

**Fremtidig hosting:** GitHub Pages
northlogiclab.github.io/TheEnginesBehind

---

## Analytiske svagheder — Del 1

### Smile Curve
**Status:** Delvist løst i v.3 — kræver eksplicit tekstforklaring
Arla må ikke ligge højere på Smile Curve end AI-infrastruktur
uden klar argumentation. AI-kurven er dybere og mere ekstrem
i begge yderpunkter. Dette skal forklares i teksten — ikke
blot vises i grafen.

### Factor Conditions Matrix
**Status:** Åben
Ratings er kvalitative vurderinger — ikke empirisk data.
Skal labelles eksplicit som konceptuel model ikke datapunkter.

---

## Åbne spørgsmål

- Skal Scandi Standard case introduceres i Del 1 eller kun Del 4?
- Skal Jon Bachs personlige positionering nævnes eksplicit i Del 1
  eller kun i Del 5?
- GitHub Pages aktivering — hvornår?

---
*Sidst opdateret: Maj 2026*
