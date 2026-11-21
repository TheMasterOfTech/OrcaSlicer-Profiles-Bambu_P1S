# 🚀 PCTG Process Profile — v5.1.0

**Bambu Lab P1S | DiamondBack 0.4 mm Nozzle | OrcaSlicer**

The PCTG 0.20 mm process profile is tuned for **peak performance** on the Bambu Lab P1S with a DiamondBack 0.4 mm nozzle.

---

## 👋 A Quick Note

It's been a while since the last public update. Profile tuning continued between releases while other projects took priority. Thanks for your patience!

---

## ✨ What's New?

### 🏗️ First-Layer Tuning

Pressure management is crucial when printing PCTG. The profile slows the first layer from **80 to 30 mm/s** and uses a minimal **two-loop skirt** on every print. The skirt primes the nozzle before it starts printing the part, giving filament flow and nozzle pressure a chance to settle. The slower first layer helps keep extrusion steady as the part begins.

| Setting | v4.2.4 | v5.1.0 |
|---|---|---|
| Initial Layer Speed | 80 mm/s | **30 mm/s** |
| Initial Layer Infill Speed | 120 mm/s | **60 mm/s** |
| Initial Layer Line Width | 0.41 mm | **0.44 mm** |
| First-Layer Flow Ratio | Inherited | **0.98** |
| Initial Layer Height | Inherited | **0.25 mm** |
| Initial Layer Print Acceleration | Inherited | **300 mm/s²** |
| Initial Layer Travel Acceleration | Inherited | **4,000 mm/s²** |
| Slow Layers | Inherited | **3** |

### 📐 Dimensional Accuracy

- Reduced elephant foot compensation from **0.10 mm to 0 mm** alongside the first-layer extrusion changes above.
- Maintained **0.005 mm XY hole compensation**.

### ⚡ Motion & Print Quality

- Reduced inner wall acceleration from **1,500 to 1,400 mm/s²** and sparse infill acceleration from **2,200 to 2,000 mm/s²**.
- Reduced internal solid infill speed from **220 to 190 mm/s** and explicitly selected **Monotonic Line** for its pattern.
- Changed the **2/4, 3/4, and 4/4** overhang speeds from **80, 70, and 60 mm/s** to **160, 120, and 80 mm/s**, respectively. The **1/4** tier now uses the inherited setting in place of the previous **100 mm/s** override.
- Set top-surface line width to **0.43 mm** and increased top-surface speed from **160 to 180 mm/s**.

### 🛠️ Supports & Slicing

- Changed the support type from **Manual Tree** to **Manual Normal**.
- Set support base pattern spacing to **1.5 mm**, interface spacing to **0.6 mm**, support angle to **45°**, and support line width to **0.44 mm**.
- Set the support/object XY distance to **0.5 mm** and the first-layer support/object gap to **0.4 mm**.
- Reduced skirt speed from **80 to 30 mm/s** and explicitly set skirt distance to **6 mm**.
- Explicitly selected the **Arachne** wall generator and reduced the small-perimeter threshold from **20 to 6 mm**.

---

## 🧵 Why 3DFuel Was Removed

Inconsistent results with 3DFuel PCTG in testing led to its removal from this release. One unverified hypothesis is that inadequate vacuum sealing allowed moisture exposure while the filament was stored at 3DFuel’s warehouse or during shipment to customers, potentially causing irreversible hydrolysis. **Atomic Filament PCTG is now currently the recommended choice.** Testing is planned for Fusion Filaments PCTG and Ambrosia’s new PCTG line.

---

## 🌡️ PCTG Bed Temperatures

Bed temperatures are tuned by build plate. The Atomic Bronze, Atomic Metallic Silver, and standalone generic PCTG presets use the same values.

| Build plate | First layer | Subsequent layers |
|---|---:|---:|
| Hot Plate | 75°C | 70°C |
| Engineering Plate | 75°C | 70°C |
| Textured PEI Plate | 70°C | 65°C |
| SuperTack Plate | 35°C | 30°C |
| Textured Cool Plate | 35°C | 30°C |
| Cool Plate | 0°C (heater off) | 0°C (heater off) |

---

## 📋 Release Information

| | |
|---|---|
| **Profile** | PCTG - 0.20mm {DB} - P1S |
| **Printer** | Bambu Lab P1S |
| **Nozzle** | DiamondBack 0.4 mm |
| **Layer Height** | 0.20 mm |
| **Previous Release** | v4.2.4 |
| **New Release** | v5.1.0 |
| **Author** | The Technical Ace (TTA) |

---

## 💬 Final Thoughts

These updates reflect ongoing refinements made through regular printing and experimentation.

As always, results may vary depending on filament, printer calibration, and environmental conditions.

**Thank you for your continued support, and happy printing! 🖨️**
