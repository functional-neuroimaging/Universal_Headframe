IIT-Rovereto Modular Mouse Headframe Clamp  
===========================================  

> A lightweight, Allen-compatible head-fixation system for imaging, electrophysiology and FUS studies  
> *Design series NT_NCS002* – by **Fabio Ricci** & **Giuliano Iurilli**, IIT Center for Neuroscience and Cognitive Systems, Rovereto (Italy), 2024 – 25

---
![323248352-13070441-1c27-4a35-8a60-9cb97c2f6576](https://github.com/user-attachments/assets/3187643e-2b83-4cff-a5cb-b85204659397)

## 1. Purpose  

Sharing mice and rigs across projects is much simpler when the mechanical interface is identical everywhere.  
This repository provides the CAD, manufacturing drawings and assembly notes for the headframe clamp we use in the Gozzi, Iurilli and Rossi labs. The clamp:

* registers a titanium headplate (≈ 1.4 g) with micron-level repeatability;  
* mates directly to standard Thorlabs Ø25 mm pillars or to a stereotaxic frame;  
* keeps the visual field unobstructed (design lineage: Allen Brain Observatory headframe);  
* survives running-mouse loads – static and dynamic deflection were bench-tested as ([P.A. Groblewski et al](https://www.sciencedirect.com/science/article/pii/S0165027020303459));  
* offers a kinematic reference that lets us reuse Allen Institute probe-positioning jigs and transparent hemisphere coordinate frames.

---

## 2. Repository layout  

```
/
├─ cad/               STEP
├─ drawings/          Dimensioned PDFs (NT_NCS002_001_P_001-004)
├─ bom/               CSV bill-of-materials
└─ images/            Renders
```

---

## 3. Bill of Materials (BoM)  

| Item | Part No. | Qty | Material | Note |
|------|----------|-----|----------|------|
| 1 | **Stereotaxic mount** NT_NCS002_001_P_001 | 1 | SS 304 | Mates to KOPF/ASI frames |
| 2 | **Top headplate clamp** NT_NCS002_001_P_002 | 1 | SS 304 | Quick-release half-bridge |
| 3 | **Bottom headplate clamp** NT_NCS002_001_P_003 | 1 | SS 304 | Matches Allen bevel | 
| 4 | **Thorlabs pillar adapter** NT_NCS002_001_P_004 | 1 | SS 304 | Ø6 mm → Ø25 mm | 
| 5 | ISO 4026 M3×5 grub-screw | 2 | - | locking pins |
| 6 | ISO 4026 M3×8 grub-screw | 1 | - | axial stop |
| 7 | ISO 4762 M3 cap-screws (various 5–20 mm) | 6 | - | assembly |  

---

## 4. Fabrication guidelines  

* **CNC milling**: 3-axis is sufficient; minimum cutter Ø 2 mm.  
* **Tolerance**: unless stated,Dimensional Tolerance class -H Geometric Tolerance class -f, General tolerancesUNI EN 22768-1 / 22768-2 UNI ISO 8015
* **Surface finish**: Ra ≤ 1.6 µm on all mating faces; tumble-debur & passivate.  
* **Headplate**: Ti-6Al-4V, 0.8 mm thick. The models in `/headplate_variants/` may be water-jet cut and bent or 3D printed by external manufacturer.  

---

## 5. Assembly & alignment workflow  

1. **Pre-load the clamp** – insert the M3 grub screws from the rear until flush.  
2. **Square to bregma** – fix the stereotaxic mount on the arm; use the printed bregma pointer to zero X/Y/Z.  
3. **Attach headplate to mouse** – follow your usual surgical SOP.  
4. **Clamp in** – slide the headplate under the bevel, tighten the single cap screw to 0.6 N m.  

---

## 6. Compatibility matrix  

| Instrument | Status | Notes |
|------------|--------|-------|
| Wide-field mesoscope | ✅ | 200 mm working distance clears clamp |
| 2-photon 10× (Nikon A1R MP) | ✅ | headplate cone variant NT_NCS002_HP-C |
| Neuropixels v1.0/v2.0 | ✅ | uses Allen transparent coordinate frame |
| Functional -Ultrasound (FUS) | 🔄 | compatible cone in prototype (M. Urosevic) |

---

## 7. License  

All hardware documentation is released under **CERN-OHL-P v2**.  
You may manufacture and modify freely; derivatives must retain the same license and attribution.

---


## 8. Acknowledgements  

* Allen Institute open-hardware programme – for the original dual-hemisphere clamp design and coordinate frame  ([Toolkit - brain-map.org](https://portal.brain-map.org/explore/toolkit/hardware?utm_source=chatgpt.com)).  
* Iurilli laboratories for beta-testing across imaging and electrophysiology

---

*Maintainer*: **Fabio Ricci** – `<fabio.ricci@iit.it>`  
