# Clasificare Imagini Reale - Salinas Construct

Acest document descrie cum sunt organizate cele **139 imagini reale** primite de la echipă (WhatsApp, 27 aprilie 2026, 18:43–18:44) și cum pot fi folosite pe site.

## Structură foldere

```
assets/photos/
├── FILENAME_MAPPING.md          # original WhatsApp filename → img_NNN.jpeg
├── CLASSIFICATION.md            # acest fișier
├── finisaje-after/              # 54 imagini cu lucrări FINALIZATE
│   ├── coridoare/   (4)         # holuri și intrări finite
│   ├── bai/         (4)         # băi moderne finite
│   ├── bucatarii/  (15)         # bucătării finalizate
│   ├── dormitoare/ (15)         # dormitoare + zonă de zi finalizate
│   └── dressinguri/(16)         # garderobe + dulapuri integrate
├── santier/         (40)        # lucrări ÎN CURS (intonacuri, instalații, demolări parțiale)
└── before-demolari/ (45)        # stadiu INIȚIAL (pereți decopertați, băi vechi, structură expusă)
```

## Cum a fost realizată clasificarea

WhatsApp salvează imaginile în ordine cronologică inversă (cele mai recente primele). Echipa a trimis fotografiile în ordine **rezultat → proces → start**:

| Interval `img_NNN` | Etapă | Conținut tipic |
|---|---|---|
| 001 – 054 | DUPĂ (`finisaje-after/`) | Spații finite: bucătării moderne, băi premium, dressinguri pe colț, holuri cu mozaic, dormitoare cu parchet englezesc |
| 055 – 094 | ÎN CURS (`santier/`) | Cartongips, intonacuri, plinte LED, montaj gresie cu nivelă laser, instalație electrică expusă, montaj centrală |
| 095 – 139 | ÎNAINTE (`before-demolari/`) | Băi vechi cu cadă albastră, pereți cu cărămidă expusă, instalații sanitare grosiere, ferestre vechi |

Limitele intervalelor au fost validate prin sondaj vizual la `img_001/005/008/010/015/020/025/030/035/040/045/050/054/055/060/065/070/075/080/085/090/094/095/100/105/110/115/120/125/130/135/139`.

## Imagini folosite în site (`index.html` → secțiune Portofoliu)

| Card | Categorie | Imagine | Subiect |
|---|---|---|---|
| 1 | renovation | `finisaje-after/bucatarii/img_010.jpeg` | Bucătărie completă cu frigider negru integrat |
| 2 | interior | `finisaje-after/bai/img_005.jpeg` | Baie modernă cu faianță bicromă și oglindă LED |
| 3 | electrical | `santier/img_085.jpeg` | Canale de cabluri în pereți de cartongips |
| 4 | renovation | `finisaje-after/coridoare/img_001.jpeg` | Coridor clasic cu mozaic alb-negru |
| 5 | plumbing | `santier/img_094.jpeg` | Centrală termică pe perete decopertat |
| 6 | interior | `finisaje-after/bucatarii/img_020.jpeg` | Bucătărie open-space cu cuptor Bosch |

## Recomandări pentru extinderea site-ului

### Sliders Înainte/După
Cele mai potrivite perechi pentru un slider Înainte/După se pot construi la nivel de **categorie** (nu la nivel de același apartament, deoarece corelarea nu este garantată):

- **Baie**: `before-demolari/img_135.jpeg` (cadă albastră veche) ↔ `finisaje-after/bai/img_005.jpeg` (baie modernă)
- **Bucătărie**: `before-demolari/img_095.jpeg` (perete cu cărămidă) ↔ `finisaje-after/bucatarii/img_010.jpeg`
- **Cameră**: `santier/img_080.jpeg` (cameră în șantier) ↔ `finisaje-after/dormitoare/img_025.jpeg`

### Galerie Servicii (modale `script.js`)
- **Renovări**: `finisaje-after/dormitoare/img_025.jpeg`, `finisaje-after/coridoare/img_001.jpeg`, `santier/img_080.jpeg`
- **Finisaje Interioare**: `finisaje-after/dressinguri/img_045.jpeg`, `finisaje-after/dormitoare/img_030.jpeg`, `finisaje-after/bucatarii/img_015.jpeg`
- **Instalații Electrice**: `santier/img_085.jpeg`, `santier/img_065.jpeg` (gresie cu laser)
- **Instalații Sanitare**: `before-demolari/img_100.jpeg` (cadru WC), `santier/img_094.jpeg`, `before-demolari/img_110.jpeg` (cartongips verde rezistent la apă)
- **Acoperișuri**: ⚠️ Nu există fotografii dedicate acoperișurilor în acest set — necesită completare separată.

### Hero Section
Imagini puternice pentru un slideshow în hero: `img_010` (bucătărie), `img_005` (baie), `img_001` (coridor), `img_025` (dormitor cu candelabru auriu).

## Note

- **Acoperișuri**: setul nu conține fotografii cu lucrări la acoperiș. Cardul "Instalații Acoperișuri" rămâne fără imagine reală până la primirea unor noi fotografii.
- **Echipă (`team-photo`)**: nu există portrete profesionale ale membrilor echipei în acest set.
- **Blog**: imaginile pot fi reutilizate pentru ilustrarea articolelor (de ex. `img_065` pentru un articol despre montaj gresie cu laser).
- Toate fișierele păstrează rezoluția WhatsApp originală (~1200px). Pentru web optim, se recomandă conversie în WebP și dimensiuni multiple (`srcset`).
