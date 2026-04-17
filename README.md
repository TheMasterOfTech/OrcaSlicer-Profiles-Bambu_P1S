# OrcaSlicer Profiles for Bambu P1S (E3D DiamondBack 0.4 mm)

These profiles are tuned specifically for the Bambu Lab P1S equipped with the E3D DiamondBack 0.4 mm integrated hotend. The goal is simple: consistent extrusion, predictable behavior, and reliable results across PCTG, PETG, PLA, and other engineering‑grade materials.

## Hardware Assumptions

Everything here is calibrated around a fixed hardware baseline so the profiles behave consistently for anyone using the same setup.

__*Printer:*__ Bambu Lab P1S with factory motion system, belts, and cooling  
__*Hotend:*__ E3D DiamondBack 0.4 mm integrated assembly  
• One‑piece sealed unit  
• No removable nozzle  
• Different melt zone and back‑pressure compared to brass or hardened steel  
__*Extruder:*__ Stock direct‑drive unit  
__*Cooling:*__ Stock part‑cooling blower and auxiliary fan  
__*Firmware:*__ Current stable release at the time of tuning  
__*AMS:*__ Optional; profiles do not rely on it  
__*Bed:*__ Stock textured PEI  
__*Environment:*__ Room ambient around 72–80 °F (22–27 °C), measured outside the enclosure

The DiamondBack is a complete hotend drop-in assembly, so all tuning values — flow, pressure advance, cooling behavior, extrusion widths, and speed limits — reflect its melt characteristics. These values won’t match what you’d expect from brass, hardened steel, or ruby nozzles.

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
├── examples/
│
├── docs/
│
└── README.md
```

## Included Profiles

This repository includes tuned **filament** and **process** profiles for the Bambu Lab P1S using a 0.4 mm DiamondBack nozzle. Filament profiles are organized by material only. Specific brands or blends will be added later as they are tuned.

### Filament Profiles
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

### Process Profiles
Located under `process/`. Currently includes PETG/PCTG‑focused profiles only:

- **PCTG & PETG – 0.20mm {DB} – P1S**

Each process profile includes:
- Speed hierarchy tuned for DiamondBack melt behavior  
- Conservative acceleration for dimensional accuracy  
- Clean seam behavior  
- Strength‑oriented infill defaults  
- No mid‑print bed temperature changes 

## How to Import

1. Download the `.ini` files you want.  
2. Open OrcaSlicer.  
3. Go to File → Import Presets.  
4. Import printer, filament, and process profiles.  
5. Restart OrcaSlicer so everything loads cleanly.

## Notes on Tuning

These profiles were built through hands‑on testing: flow calibration, pressure advance sweeps, cooling curve checks, extrusion width validation, and dimensional accuracy tests. The DiamondBack’s thermal stability and wear resistance make it extremely consistent, but its melt characteristics differ from traditional nozzles. Expect different PA and flow values if you’re coming from brass or hardened steel.

## License

MIT License — free to use, modify, and share with attribution.
