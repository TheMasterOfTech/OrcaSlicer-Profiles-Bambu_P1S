# OrcaSlicer Profiles for Bambu P1S (E3D DiamondBack 0.4 mm)

These profiles are tuned specifically for the Bambu Lab P1S equipped with the E3D DiamondBack 0.4 mm integrated hotend. The goal is simple: consistent extrusion, predictable behavior, and reliable results across PCTG, PETG, PLA, and other engineering‑grade materials.

## Hardware Assumptions

Everything here is calibrated around a fixed hardware baseline so the profiles behave the same way for anyone using the same setup.

Printer: Bambu Lab P1S with factory motion system, belts, and cooling  
Hotend: E3D DiamondBack 0.4 mm integrated assembly  
• One‑piece sealed unit  
• No removable nozzle  
• Different melt zone and back‑pressure compared to brass or hardened steel  
Extruder: Stock direct‑drive unit  
Cooling: Stock part‑cooling blower and auxiliary fan  
Firmware: Current stable release at the time of tuning  
AMS: Optional; profiles do not rely on it  
Bed: Stock textured PEI  
Environment: Room ambient around 72–80 °F (22–27 °C), measured outside the enclosure

Because the DiamondBack is a complete hotend assembly, all tuning values — flow, pressure advance, cooling behavior, extrusion widths, and speed limits — reflect its melt characteristics. They won’t match what you’d expect from brass, hardened steel, or ruby nozzles.

## Included Profiles

Printer presets tuned for the DiamondBack’s melt behavior  
Filament presets with calibrated flow, cooling, and PA  
Process presets focused on dimensional accuracy, strength, and repeatability

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
