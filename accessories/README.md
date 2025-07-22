# Universal\_Headframe ─ Accessories Library 
Welcome!  This repository collects every **Accessories** we currently use or test at IIT Rovereto.  Each model comes as a STEP file (`.step`) ready for CAM / 3‑axis milling, direct metal‑AM printing, or SLA 3D printin, plus a PNG preview so you can eyeball the geometry before downloading CAD.

> **TL;DR**  • All files are **metric** (ISO M‑series screws, millimetres).

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
| `0160-073-01_FR.step`        |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/d9629387-1684-4be4-83f3-da9fcd6184ba" /> | xx g | x mm       | **Allen institute lineage** 	titanium headframe utilized with the [SHIELD]( https://cad.onshape.com/publications/a9da3d5bea6057b1de9dcbe4/w/e8fb183696b8dd84a43603fb/e/8e9294519ca4564a8390c596?renderMode=0&leftPanel=false&uiState=687e53a48cc3d5295ef9be1f ) implant for dual hemisphere electrophysiological recordings|
| `DHC Stamp Tool_Stamp_tool_DH_FR.step`|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/737602b0-636a-4b25-b1ce-7d8e50378b73" />| xx  g | x mm       | **Allen institute lineage**  Headframe-shank mounted stylus for setting stereotax clamp location with respect to Bregma|
| `Stamp_tool_SH_FR.step`        |<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/52fde1f3-948a-418d-be3b-6fbe77c8fc69" />| xx g | x mm        |**Allen institute lineage**Headframe-shank mounted Whole Hemisphere Implant Tracer |
| `AH_USSEnterprise_cone_FR.step`|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/b2470306-d3b9-465a-a05c-f2e43692bdff" />| xx g | x mm        | **Skull‑contoured** geometry—full compatibility, acute imaging, [SHIELD]( https://cad.onshape.com/publications/a9da3d5bea6057b1de9dcbe4/w/e8fb183696b8dd84a43603fb/e/8e9294519ca4564a8390c596?renderMode=0&leftPanel=false&uiState=687e53a48cc3d5295ef9be1f ) implant for dual hemisphere electrophysiological recordings |
| `AH_USSEnterprise_cover.step`|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/56db0925-8883-4969-b1a7-c4388b0afbe0" />| xx g | x mm       | Headframe-shank mounted Dual Hemisphere Implant Tracer       			           |
| `Luigi_cone.step`|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/45404b41-67d2-434d-981d-b1479ca10d60" />| xx g | x mm       | Plate with keyed seat for Eppendorf to insert NP2 shanks            |
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
