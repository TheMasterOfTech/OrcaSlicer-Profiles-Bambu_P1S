# OrcaSlicer Profiles for Bambu P1S
[![Latest Release](https://img.shields.io/github/v/release/TheMasterOfTech/OrcaSlicer-Profiles-Bambu_P1S?label=Latest%20release&color=0A3C7D&style=for-the-badge)](https://github.com/TheMasterOfTech/OrcaSlicer-Profiles-Bambu_P1S/releases)
### ⚠️ Utilizes an E3D DiamondBack 0.4 mm nozzle/hotend assembly

These profiles are tuned specifically for the Bambu Lab P1S equipped with the E3D DiamondBack 0.4 mm integrated hotend. With rigorous and passionate testing, consistent extrusion, predictable behavior, and reliable results across PCTG, PETG, PLA, and other engineering‑grade materials is provided with these profiles.

The DiamondBack is a complete hotend drop-in assembly, so all tuning values (flow, pressure advance, cooling behavior, extrusion widths, and speed limits) reflect its melt characteristics. As such, it is expected that these values won’t match what you’d expect from brass, hardened steel, or ruby nozzles.

## Hardware Setup & Environment

__*Printer:*__ Bambu Lab P1S with factory motion system, belts, and cooling <br>
__*Hotend:*__ E3D DiamondBack 0.4mm (complete hotend) <br>
• One‑piece sealed unit  
• No removable nozzle  
• Different melt zone and back‑pressure compared to brass or hardened steel <br>
__*Build Surface:*__ [West3D Black Textured PEI](https://west3d.com/products/bambu-double-sided-texture-black-pei-pro-by-west3d)<br>
__*Extruder:*__ Stock direct‑drive unit  
__*Cooling:*__ Stock part‑cooling blower and auxiliary fan  
__*Firmware:*__ Current stable release at the time of tuning  
__*AMS:*__ Optional; profiles do not rely on it  
__*Bed:*__ Stock textured PEI  
__*Environment:*__ Room ambient around 72–80 °F (22–27 °C), measured outside the enclosure


## GitHub Repository Layout
```
orcaslicer-profiles-bambu_p1s/
│
├── filament/
│   ├── PLA/
│   ├── PETG/
│   ├── PCTG/
│   └── ASA/
│
├── process/
│
├── RELEASE_NOTES.md
│
└── README.md
```

## Filament & Process Profiles

This repository includes tuned **filament** and **process** profiles for the Bambu Lab P1S using a 0.4 mm DiamondBack nozzle. Filament profiles are organized by material only. Specific brands or blends will be added later as they are tuned if found necessary.

<details>
<summary><strong>Filament Profiles</strong></summary>

<br>

Located under `filament/`, organized by material:

- **PLA**
- **PETG**
- **PCTG**
- **ABS**

Each filament profile includes:
- Flow ratio tuned for DiamondBack melt behavior  
- Pressure advance values validated through real prints  
- Cooling assumptions appropriate for the enclosed P1S  
- Consistent extrusion width logic across materials  

</details>

<details>
<summary><strong>Process Profiles</strong></summary>

<br>

Located under `process/`.

- **PCTG – 0.20mm {DB} – P1S**

Each process profile includes:
- Speed hierarchy tuned for DiamondBack melt behavior  
- Conservative acceleration for dimensional accuracy  
- Clean seam behavior  
- Strength‑oriented infill defaults  
- No mid‑print bed temperature changes  

</details>

### How to Import

1. Download the `OrcaSlicer-Profiles-Bambu_P1S.zip` file from the [latest release](https://github.com/TheMasterOfTech/OrcaSlicer-Profiles-Bambu_P1S/releases).
2. Open OrcaSlicer.  
3. Go to **File** → **Import Presets**.  
4. Import printer, filament, and/or process profiles that you wish to (they end in `.ini`).
5. Restart OrcaSlicer so everything loads cleanly.

## Friendly Advisories

These profiles were built through hands‑on testing: flow calibration, pressure advance (PA) sweeps, cooling curve checks, extrusion width validation, bridging tests, and dimensional accuracy verification. The DiamondBack’s thermal stability and wear resistance make it extremely consistent, but its melt characteristics differ from traditional nozzles. Expect different PA and flow values if you’re coming from brass or hardened steel.

Respectfully, I will not be developing profiles for slicers outside of OrcaSlicer (such as Bambu Studio or PrusaSlicer). I exclusively use OrcaSlicer for all of my printers, and it isn’t practical for me to allocate time to maintain profiles for additional slicers. However, you’re welcome to message me if you’d like guidance on developing your own profiles for those platforms.

## License

MIT License — free to use, modify, and share with attribution.
