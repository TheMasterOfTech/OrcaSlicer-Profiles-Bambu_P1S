# OrcaSlicer Profiles for Bambu P1S (E3D DiamondBack 0.4 mm)

A collection of empirically tuned OrcaSlicer profiles for the Bambu Lab P1S, calibrated specifically for the E3D DiamondBack 0.4 mm integrated hotend assembly. These profiles prioritize consistency, dimensional accuracy, and repeatable results across PCTG, PETG, PLA, and engineering filaments.

---

## Hardware Assumptions

All profiles in this repository are tuned against a fixed, controlled hardware baseline to ensure consistent and reproducible behavior. Every flow, pressure advance, cooling, and extrusion parameter assumes the following setup:

- **Printer:** Bambu Lab P1S (factory motion system, stock belts, stock fans)
- **Hotend Assembly:** E3D DiamondBack 0.4 mm — full integrated unit  
  - This is a single-piece, sealed DiamondBack hotend  
  - The nozzle is permanently integrated and cannot be removed or swapped  
  - Melt zone length, thermal behavior, and back-pressure differ from brass, hardened steel, and ruby nozzles
- **Extruder:** Stock P1S direct-drive extruder
- **Cooling:** Stock part-cooling blower and auxiliary fan
- **Firmware:** Current stable Bambu Lab firmware at the time of tuning
- **AMS:** Optional; profiles do not assume AMS usage
- **Bed:** Stock textured PEI plate unless otherwise noted
- **Environment:** Room ambient around 72–80°F (22–27°C), measured *outside* the printer enclosure

Because the DiamondBack is a fully integrated hotend, all tuning values in this repository—flow ratio, pressure advance, cooling percentages, extrusion widths, and speed limits—are calibrated specifically for the DiamondBack’s extrusion characteristics and should not be expected to behave identically on other nozzle or hotend types.

---

## Included Profiles

This repository contains:

- **Printer Profiles**  
  Tuned for the DiamondBack’s melt characteristics and extrusion behavior.

- **Filament Profiles**  
  Flow ratio, cooling, and PA calibrated per material.

- **Process Profiles**  
  Layer height, extrusion width, speed, and strength presets optimized for reliability and dimensional accuracy.

---

## How to Import

1. Download the `.ini` files from this repository.  
2. Open OrcaSlicer.  
3. Go to **File → Import Presets**.  
4. Import printer, filament, and process profiles as needed.  
5. Restart OrcaSlicer to ensure all presets load correctly.

---

## Notes on Tuning

These profiles were developed through iterative empirical testing, including:

- Flow ratio calibration  
- Pressure advance tuning  
- Cooling curve validation  
- Extrusion width and speed stability checks  
- Strength and dimensional accuracy verification  

The DiamondBack’s thermal stability and reduced wear allow for highly consistent extrusion, but its melt characteristics differ from brass and hardened steel. Users switching from non‑DiamondBack hotends should expect different PA and flow values.

---

## License

MIT License — free to use, modify, and share with attribution.
