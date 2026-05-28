# SIA "Kultūras centrs" — projekta konteksts

## Uzņēmums

| Lauks | Vērtība |
|-------|---------|
| Nosaukums | SIA "Kultūras centrs" |
| Reģ.nr. | 40103381801 |
| Juridiskā adrese | Skolas iela 15, Rīga, LV-1010 |
| Reģistrēts | 2011-02-16 |
| Valdes loceklis | Kaspars Kondratjuks |
| Grāmatvedis | Signe Silova / SIA "Laimes Brīdis" (40103759132) |

## Faili šajā repozitorijā

| Fails | Apraksts |
|-------|----------|
| `2025_gada_parskata_skaidrojums.md` | **Avota fails.** 2025. gada pārskata skaidrojums latviski. Rediģē šeit; pēc tam sinhronizē ar HTML. |
| `2025_gada_parskata_skaidrojums.html` | HTML versija dalīšanai ar līdzīpašniekiem/kreditoriem. Derivāts no MD. |
| `KC_uznemuma_vertejums.html` | Interaktīvs vērtējuma rīks (vanilla JS + Chart.js CDN). Standalone `file://` vai GitHub Pages. |
| `SIA_KC_Shareholder_Overview.md` | Iepriekšējais līdzīpašnieku pārskats (maijs 2026). Kontekstuāls, nav primārs. |
| `data/kc_2025_facts.json` | Vienots datu avots — visi 2025. gada skaitļi ar avotu atsaucēm. Atjaunini šeit, tad propagē uz HTML. |
| `data/external_valuation_extract.md` | Ārējā vērtētāja DCF modeļa izvilkums (2024-05, `Finanšu modelis.xlsx`). |
| `index.html` | GitHub Pages sākumlapa ar saitēm uz abiem HTML failiem. |
| `KKc bussiness.md` | **PRIVĀTS — .gitignore.** Raw stratēģiskās diskusijas ar individuālo pušu vārdiem. Nekad nepublicē. |

## Redakcijas darba plūsma

- **Teksta izmaiņas** → rediģē `2025_gada_parskata_skaidrojums.md`, tad sinhronizē ar HTML versiju
- **Skaitļu korekcijas** → atjaunini `data/kc_2025_facts.json`, tad propagē uz HTML
- **Vērtējuma rīka loģika** → rediģē `KC_uznemuma_vertejums.html` tieši (JS objekts `DATA` lapas augšā)
- Pēc izmaiņām: `git add -p && git commit && git push` → GitHub Pages atjaunojas automātiski (~1 min)

## GitHub Pages

- **Publiska URL:** `https://kasparkondrat.github.io/sia-kulturas-centrs/`
- Repozitorijs ir **publisks** — nepublicē sensitīvu informāciju (individuālo kreditoru dati, stratēģiskās sarunas)
- `.gitignore` bloķē `KKc bussiness.md` un `~$*` (Office lock faili)

## Galvenie 2025. gada finanšu dati

Avots: `data/kc_2025_facts.json` + `GP/2025/Kultūras centrs_gada pārskats.pdf` (parakstīts 2026-05-14)

| Rādītājs | 2025 | 2024 |
|----------|-----:|-----:|
| Apgrozījums | €117,160 | €85,993 |
| Neto rezultāts | -€19,814 | -€69,532 |
| Pašu kapitāls | -€22,376 | -€2,563 |
| Ilgtermiņa aizņēmumi | €431,711 | €440,317 |
| Bilance kopā | €443,497 | €475,366 |
| Nauda | €3,022 | €1,502 |

## Aizdevumi (pēc 2026-05-13 vienošanās)

| Kreditors | Pamatsumma | Mēneša maksājums | Termiņš | Procenti |
|-----------|----------:|----------------:|---------|---------|
| SALMO/GV | €250,000 | €2,700 pamatsumma | 92 mēn (~2034-01) | 4%/gadā, balloon |
| Rododendri | €182,000 | ~€1,978 pamatsumma | 92 mēn (~2034-01) | 4%/gadā, balloon |
| Off-books | €66,911 | €0 | Nav grafika | 0% |

Procenti tiek uzkrāti grāmatvedībā bet nav jāmaksā naudā līdz aizdevuma perioda beigām (~€60-80k balloon 2034).

## Strukturālā maiņa 2026-06-01

Trīs jauni līgumi (parakstīti 2025-09-29 līdz 2025-12-15):

1. **KC → KLKC pirkuma līgums (29.09.2025):** būvprojekts BV-19-557-abu/V pārdots par €1,000 + PVN
2. **FL → KLKC nomas līgums (30.09.2025):** KLKC tieši nomā 2. un 3. stāvu no FL, €1,869.40/mēn, līdz 2041-05-01
3. **Vienošanās Nr.2 KC ↔ FL (15.12.2025):** KC nomā tikai 1F + pagrabs (246.68 m²) + 607 m² zemes, €862.93/mēn, līdz 2041-05-01

Neto ietekme uz KC: nomas izmaksas samazinās par €22,433/gadā; KLKC nomas pārrēķins pazūd no ieņēmumiem; EBITDA paliek ~€59-65k/gadā.

Vienošanās Nr.2 satur **ieguldījumu kompensācijas klauzulu** (FL pārkāpuma gadījumā KC saņem atpakaļ ieguldījumus — summa jāaizpilda, atsaucoties uz €405,711 bilancē). Drošības naudas atgriešanas % arī palicis tukšs — jāprecizē ar FL.

## Ārpākalpojuma grāmatvedis kontakts

- **Signe Silova** — primārais kontakts jautājumiem par bilanci, procentu uzkrāšanas detalizāciju, €66,911 off-books kvalifikāciju
- SIA "Laimes Brīdis", reģ.nr. 40103759132

## Ārējais vērtējums (salīdzināšanai)

`Finanšu modelis.xlsx` (lokālais fails, ~2024-05, ārējais konsultants):
- WACC 6.01%: equity €1,388,005
- WACC 8.57%: equity €616,045
- **Pieņēmumi atšķiras no realitātes** — modelēja visu stāvu komerciālu iznomāšanu, nevis Sarūsējis 1F modeli

## Saistītie avota faili (Google Drive, nav repozitorijā)

- `KKC/KC SIA/GP/2025/` — oficiālais gada pārskats (PDF + edoc), bilances XLSX, PZA XLSX
- `KKC/KC SIA/Finanses/` — finanšu modeļi, scenāriji 2026-2041
- `KKC/KC SIA/Fraternitas Lettica/LĪGUMS/ORIĢINĀLI/7_WIDEN_JAUNI_LĪGUMI_100925/` — visi 2025. gada jaunie līgumi
