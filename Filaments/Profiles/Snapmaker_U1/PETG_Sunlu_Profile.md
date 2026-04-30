# SUNLU PETG – Snapmaker U1 Profile

## 🖨 Setup
- Printer: Snapmaker U1
- Slicer: OrcaSlicer
- Material: SUNLU PETG

---

## 📊 Included
- Adaptive Pressure Advance testing
- Flow calibration (in progress)

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

See detailed analysis:  
[Adaptive PA Table](../../Filaments/PETG/Sunlu/adaptive_PA_table.md)

---

## 🔧 Status
⚠️ Profile currently in progress.

---

### Current Focus
- Validate layer adhesion from layer 2 upward
- Optimize low-flow PA behavior

---

## 💡 Notes
This profile is being developed based on real-world testing and structured calibration.

Final values will be added soon.
