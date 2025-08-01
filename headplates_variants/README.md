# Universal\_Headframe ─ Variant Library 
Welcome!  This repository collects every **head‑plate variant** we currently use or test at IIT Rovereto.  Each model comes as a STEP file (`.step`) ready for CAM / 3‑axis milling, direct metal‑AM printing, or SLA 3D printin, plus a PNG preview so you can eyeball the geometry before downloading CAD.

> **TL;DR**  • All files are **metric** (ISO M‑series screws, millimetres). • Default material is **Ti‑TC4** (works in SLM or CNC), some of them can be made in plastic.

---

## How this README is organised

| Section                                 | What you’ll find                              |
| --------------------------------------- | --------------------------------------------- |
| [Quick chooser](#quick-chooser-table)   | one‑line guide to pick the right plate        |
| [Fabrication notes](#fabrication-notes) | tips for CNC vs SLM printing                  |

---

## Quick chooser table

| File name                    | Preview                                           | Mass\* | Aperture Ø | Typical use‑case                                                         |
| ---------------------------- | ------------------------------------------------- | ------ | ---------- | ------------------------------------------------------------------------ |
| `0160-075-00_FR.step`        |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/d9629387-1684-4be4-83f3-da9fcd6184ba" /> | xx g | x mm       | **Allen institute lineage** 	titanium headframe utilized with the [SHIELD](http://cad.onshape.com/publications/a9da3d5bea6057b1de9dcbe4/) implant for dual hemisphere electrophysiological recordings|
| `0251-900-04_FR.step`        |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/737602b0-636a-4b25-b1ce-7d8e50378b73" />| xx  g | x mm       | **Allen institute lineage**  Headframe-shank mounted stylus for setting stereotax clamp location with respect to Bregma|
| `0251-910-00_FR.step`        |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/52fde1f3-948a-418d-be3b-6fbe77c8fc69" />| xx g | x mm        |**Allen institute lineage**Headframe-shank mounted Whole Hemisphere Implant Tracer |
| `AH_USSEnterprise_FR.step`   |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/b2470306-d3b9-465a-a05c-f2e43692bdff" />| xx g | x mm        | **Skull‑contoured** geometry—full compatibility, acute imaging, [SHIELD](http://cad.onshape.com/publications/a9da3d5bea6057b1de9dcbe4/) implant for dual hemisphere electrophysiological recordings |
| `DHC Tracer_FR.step`         |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/56db0925-8883-4969-b1a7-c4388b0afbe0" />| xx g | x mm       | Headframe-shank mounted Dual Hemisphere Implant Tracer       			           |
| `Eppendorf_FR.step`          |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/45404b41-67d2-434d-981d-b1479ca10d60" />| xx g | x mm       | Plate with keyed seat for Eppendorf to insert NP2 shanks            |
| `Luigi_Headplate_V1_FR.step` |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/6ceb3b4a-dbaf-4a54-848c-202b832a638d" />| xx g | x mm       | Luigi petrucco variant Ephys|
| `0160-055-00_X01_FR.step`    |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/b7f07272-9334-41a1-8d5c-6cd5b2c36aa6" />| xx g | x mm       | variant.                |
| `0160-073-00_A_FR.step`      |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/6c8d0bb0-3c38-4c7e-b21b-645305a426ff" />| xx g | x mm       | **Allen institute lineage** 	titanium headframe utilized with the [SHIELD](http://cad.onshape.com/publications/a9da3d5bea6057b1de9dcbe4/) implant for whole hemisphere electrophysiological recordings - Version 2 - Ring style.|

<sub>\*Mass values are printed Ti‑TC4 as measured on a 0.1 mg balance</sub>

---

## Fabrication notes

* **3‑D printing (SLM)** – upload to JLC3DP or similar; choose **Ti‑TC4** and "high precision" option if offered.
* **CNC milling** – water‑jet or laser‑cut 1.6 mm Ti sheet, then finish on 3‑axis mill;
* **3-D printing  (SLA)** - Used a Form 2 for parts that does not endure loads.

---


### Contributing

Pull requests welcome—open an issue if you have a new variant or measurement data to share.

### License

CERN-OHL-P-2.0 license.
