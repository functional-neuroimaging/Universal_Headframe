# (Just a template for chat GPT, do not read)
# Universal\_Headframe ─ Variant Library 
Welcome!  This repository collects every **head‑plate and clamp variant** we currently use or test at IIT Rovereto.  Each model comes as a STEP file (`.step`) ready for CAM / 3‑axis milling or direct metal‑AM printing, plus a PNG preview so you can eyeball the geometry before downloading CAD.

> **TL;DR**  • All files are **metric** (ISO M‑series screws, millimetres). • Default material is **Ti‑TC4** (works in SLM or CNC), some of them can be made in plastic.

---

## How this README is organised

| Section                                 | What you’ll find                              |
| --------------------------------------- | --------------------------------------------- |
| [Quick chooser](#quick-chooser-table)   | one‑line guide to pick the right plate        |
| [Variant gallery](#variant-gallery)     | bigger screenshots + design notes             |
| [Fabrication notes](#fabrication-notes) | tips for CNC vs SLM printing                  |
| [FAQ](#faq)                             | common questions about mass, clearances, etc. |

---

## Quick chooser table

| File name                    | Preview                                           | Mass\* | Aperture Ø | Typical use‑case                                                         |
| ---------------------------- | ------------------------------------------------- | ------ | ---------- | ------------------------------------------------------------------------ |
| `0160-100-57_FR.step`        | ![0160‑100‑57](img/0160-100-57_FR.png)            | xx g | x mm       | **Flat, lightweight** Ti plate for chronic Neuropixels recordings        |
| `0251-900-04_FR.step`        | ![0251‑900‑04](img/0251-900-04_FR.png)            | xx  g | x mm       | **Skull‑contoured** version for reduced profile under wide‑field scopes  |
| `0251-910-00_FR.step`        | ![0251‑910‑00](img/0251-910-00_FR.png)            | xx g | x mm      | **Large‑window** plate for mesoscope & wide FOV 2‑P                      |
| `AH_USSEnterprise_FR.step`   | ![AH USS Enterprise](img/AH_USSEnterprise_FR.png) | xx g | x mm      | **Skull‑contoured** geometry—full compatibility, acute imaging |
| `DHC Tracer_FR.step`         | ![DHC Tracer](img/DHC%20Tracer_FR.png)            | xx g | x mm       | for tracer        			           |
| `Eppendorf_FR.step`          | ![Eppendorf](img/Eppendorf_FR.png)                | xx g | x mm       | Plate with keyed seat for Eppendorf to insert NP2 shanks            |
| `Luigi_Headplate_V1_FR.step` | ![Luigi V1](img/Luigi_Headplate_V1_FR.png)        | xx g | x mm       | **Front attached** Luigi variant                   |
| `0160-055-00_X01_FR.step`    | ![0160‑055‑00](img/0160-055-00_X01_FR.png)        | xx g | x mm       | **Dual‑probe** variant—clearance slots for bilateral NP2                 |
| `0160-073-00_A_FR.step`      | ![0160‑073‑00](img/0160-073-00_A_FR.png)          | xx g | x mm       | **FUS‑ready**: recessed window for 15 MHz transducer alignment           |

<sub>\*Mass values are printed Ti‑TC4 as measured on a 0.1 mg balance</sub>

---

## Variant gallery

### 0160‑100‑57 — Flat lightweight plate

![0160‑100‑57](img/0160-100-57_FR_large.png)

* **Why**: our default chronic plate where <0.5 g total load is required.
* **Clamp**: single M2 cap‑screw into V‑block; mirror‑finish datum nose for sub‑µm repeatability.

### 0251‑900‑04 — Skull‑contoured

![0251‑900‑04](img/0251-900-04_FR_large.png)

* Matches average C57BL/6 skull curvature to drop objective‑to‑cortex distance by \~1 mm.
* Good for wide‑field macrosopes that need WD ≈35 mm.

### 0251‑910‑00 — Large‑window / mesoscope

![0251‑910‑00](img/0251-910-00_FR_large.png)

* 10 mm aperture pairs with UCLA Mesoscope or ASI v3 large NA lenses.
* Comes with printable dust‑cap for long‑term chronic windows.

### AH\_USSEnterprise — Allen reference plate

![AH USS Enterprise](img/AH_USSEnterprise_FR_large.png)

* Full Allen kinematic coupler and 3‑pin datum—max stability, but heavier.
* Imperial version converted to **M2/M3** for EU sourcing.

### DHC Tracer

![DHC Tracer](img/DHC%20Tracer_FR_large.png)

* Rear tower accepts 23–33 g syringe holder for iontophoretic tracers.
* Maintains <0.55 g by thinning front web.

### Eppendorf

![Eppendorf](img/Eppendorf_FR_large.png)

* Quick‑dock for Eppendorf FemtoJet nano‑injector nosepiece.
* Slots for z‑index pins so you can swap animals without recalibrating depth.

### Luigi Headplate V1

![Luigi V1](img/Luigi_Headplate_V1_FR_large.png)

* Featherweight training plate to habituate juvenile mice.
* Clamp mounts backward‑compatible with all rigs in this repo.

### 0160‑055‑00\_X01 — Dual‑probe

![0160‑055‑00](img/0160-055-00_X01_FR_large.png)

* Left + right slots line up with NP2 baseplates at 15° pitch.
* Comes with parametric jig for pre‑drill in OpenSCAD.

### 0160‑073‑00\_A — FUS ready

![0160‑073‑00](img/0160-073-00_A_FR_large.png)

* 2 mm recess holds silicone coupling cone; tested to 15 MHz FUS.
* Window ring screws on after ultrasound session.

---

## Fabrication notes

* **3‑D‑printing (SLM)** – upload to JLC3DP or similar; choose **Ti‑6Al‑4V** and "high precision" option if offered. Support scars lie on the underside; easy to sand flat.
* **CNC milling** – water‑jet or laser‑cut 0.4 mm Ti sheet, then finish on 3‑axis mill; bend radius ≥0.25 mm.
* **Datum finishing** – lap the V‑groove and nose on 2000‑grit + diamond paste for micron‑level repeatability.

---

## FAQ

<details><summary>Why not aluminium for ultra‑light?</summary>
Al is light but its Young’s modulus is ~70 GPa vs Ti’s 110 GPa; the same 0.4 mm plate deflects ~1.5× more. For chronic rigs that extra flex shows up as motion artefact.
</details>

<details><summary>Can I switch back to imperial screws?</summary>
Sure—parametric CAD lets you flip hole diameters + thread models in seconds. We default to metric to keep EU machining simple.
</details>

<details><summary>What about plastics / PEEK?</summary>
Great for geometry prototypes, but stiffness / creep are limiting for month‑long implants unless you bulk up the thickness and accept extra mass.
</details>

---

### Contributing

Pull requests welcome—open an issue if you have a new variant or measurement data to share.

### License

BSD‑3‑Clause.  Use freely, cite the repo if you publish.
