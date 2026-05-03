# SUNLU PETG – Snapmaker U1 Profile

## Version

**v0.1 – Initial Release (Work in Progress)**

## 🖨 Setup
- Printer: Snapmaker U1
- Slicer: OrcaSlicer
- Material: SUNLU PETG

---

## 📥 Download

👉 [Download Profile](SUNLU_PETG_U1_v0.1.orca.zip)
👉 [Download Profile](https://raw.githubusercontent.com/RicoBandito/Rico3D-Profiles/main/Filaments/Profiles/Snapmaker_U1/SUNLU_PETG_U1_v0.1.orca.zip)

---

## ⚙️ Current Settings (Test State)

### Context

These values are the result of flow and pressure advance calibration.  
They are not considered final and may change based on ongoing validation.

- Global Flow: 0.91
- Global PA: 0.025
- Max Volumetric Speed: 14.5 mm³/s

Adaptive PA:  
See detailed table:
[Adaptive PA Table](../../Filaments/PETG/Sunlu/adaptive_PA_table.md)

---

## 📊 Included
- Adaptive Pressure Advance testing
- Flow calibration (in progress)

---

## ✅ Recommended Use

- General PETG printing (tested baseline)
- PETG support interface for PLA
- Mixed material support scenarios (PLA ↔ PETG)

⚠️ Not yet optimized for:
- High-speed production prints
- Maximum strength parts (layer adhesion under validation)

---

## ⚠️ Known Issue – Layer Adhesion

Layer adhesion issues were observed beyond the first layer.

### Observation
- First layer improved with Z-offset adjustment
- Issue reappeared from layer 2 onwards

### Suspected Cause
Adaptive Pressure Advance behavior in low volumetric flow regions may cause under-extrusion during critical bonding phases.

### Current Approach
- Reduce low-flow PA values
- Validate bonding improvement
- Maintain surface quality

See detailed analysis in the Adaptive PA section above.

---

## 🔧 Status
⚠️ Profile currently in active development and validation phase.

---

### Current Focus
- Validate layer adhesion from layer 2 upward
- Optimize low-flow PA behavior

---

## 💡 Notes
This profile is being developed based on real-world testing and structured calibration.

Final values will be added soon.

## 📜 Changelog

### v0.1
- Initial structured profile
- Adaptive PA system implemented
- Layer adhesion issue identified and under investigation

---#

## 🎯 Goal

Build a reliable, reproducible PETG profile with:
- consistent layer adhesion
- stable adaptive PA behavior
- cross-material compatibility
