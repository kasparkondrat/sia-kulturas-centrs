# Ārējā vērtētāja modeļa izvilkums

**Avots:** `KKC/KC SIA/Finanses/Finanšu modelis.xlsx` (lokālā kopija — saturs identisks gsheet `1nQWwFpxTtaN99QOhpo8wDYH6zCZOV5nXGaDJZvFo77E`)
**Modeļa datums:** ~2024-05 (atskaites datums "31.05.2024")
**Lapas:** Modelis, DCF aprēķins

## Galvenie pieņēmumi (ņemti no DCF lapas)

| Parametrs | Vērtība | Avots |
|-----------|---------|-------|
| Bezriska likme (Rf) | 2.7% | 10Y EU Eurobond yield, May 2024 |
| Nozares beta (asset, unlevered) | 0.41 | Damodaran 2024, Real Estate General |
| Valsts riska prēmija (Latvija) | 1.75% | Damodaran 2024 |
| UIN likme | 25% | LR likums |
| Procentu likme parādam | 4% | Klienta sniegta info |
| Ilgtermiņa pieauguma likme | 3% | LR EM ilgtermiņa GDP prognoze |
| Pamatkapitāls (esošais) | €47,222 | Bilance |
| Parāda atlikums | €392,517 | Bilance 31.05.2024 |
| Naudas atlikums | €5,110 | Bilance 31.05.2024 |

## Biznesa modelis (kas tika modelēts)

Ārējais vērtētājs modelēja scenāriju, KAS ATŠĶIRAS no pašreizējās realitātes:
- Visi 4 stāvi tiek iznomāti komerciāli (pagrabs €5/m², 1.st €15/m², 2-3.st €13/m², terase €5/m²)
- Vidējā telpu noslodze: 75%
- Īres cenu kāpums: 5%/gadā
- Renovācijai jauns aizdevums €260,000 (96 mēn termiņš)
- Esošā aizdevuma atmaksa €105,315/gadā (~€8,776/mēn)
- Amortizācija €90,000/gadā (lielas investīcijas ar 8 gadu nolietojuma periodu)

Reālie 2025. gada dati no oficiālā gada pārskata:
- Apgrozījums: €117,160 (vs prognozēts €94,410 — **24% AUGSTĀKS**)
- Bet uz citu darbības modeli — Sarūsējis īrē tikai 1. stāvu + pagrabu, KLKC pārvalda 2-3. stāvu (atsevišķa nelegālā vienība)

## DCF rezultāti — divas iterācijas

### 1. iterācija (CAPM ar grāmatvedības pašu kapitālu)
- WACC: **6.01%**
- 10 gadu DCF (2025-2034): €131,205
- Terminal value: €1,644,207
- Pašu kapitāla (100%) vērtība: **€1,388,005**

### 2. iterācija (CAPM ar tirgus pašu kapitālu = 1.iterācijas rezultāts)
- WACC: **8.57%**
- 10 gadu DCF: €100,353
- Terminal value: €903,100
- Pašu kapitāla (100%) vērtība: **€616,045**

## Mūsu komentārs

Ārējais vērtējums **strukturāli pareizs**, bet:
1. **Modelēts cits biznesa modelis** (visu stāvu komerciāla iznomāšana) — neatbilst pašreizējai realitātei pēc 2024. gada strukturālajām izmaiņām ar Sarūsējis un KLKC
2. **Pieņemtais EBITDA** (€91k 2025., augot līdz €142k 2034.) ir augstāks par to, ko sasniegs jaunais modelis (Scenario 2: €59-65k stabils EBITDA)
3. **WACC pieņēmumi pamatoti** ar uzticamiem avotiem (Damodaran, ECB)
4. **Galvenais ieskats no ārējā vērtējuma:** uzņēmuma vērtība ir augsta tieši TĀPĒC, ka tas tur **galveno nomas līgumu ar Fraternitas Lettica** — tas ir vērtīgs ilgtermiņa aktīvs neatkarīgi no operatīvā modeļa

## Atjaunināts vērtējums ar 2025. gada faktiem

Ja izmantojam to pašu WACC metodiku (6-8.6% diapazonu) ar **reālistisku** Scenario 2 naudas plūsmu (€59-65k EBITDA stabils):

- DCF (10 gadi 2026-2036, vidēji €60k EBITDA): ~€440-500k
- Terminal value (3% pieaugums, 6-8% WACC): €590k - €1.1M
- Enterprise Value: €1.0 - €1.6M
- Equity Value (EV − parāds €432k): €570k - €1.17M

Šis aptuvenais aprēķins atbilst ārējā vērtētāja 2. iterācijas rezultātam (€616k) — ar atšķirību, ka vērtība galvenokārt nāk no nomas līguma turēšanas, nevis no augstas operatīvās peļņas.
