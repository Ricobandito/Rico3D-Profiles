# SUNLU PETG – Snapmaker U1 Profile

## 🖨 Setup
- Printer: Snapmaker U1
- Slicer: OrcaSlicer
- Material: SUNLU PETG

---

## 🔧 Status
⚠️ Profile currently in progress.

## ⚠️ Known Issue – Layer Adhesion

Layer adhesion issues were observed beyond the first layer.

### Root Cause (suspected)
Adaptive Pressure Advance causing under-extrusion in low flow regions.

### Observation
- First layer improved via Z-offset
- Issue persisted in upper layers

### Current Fix Strategy
- Reducing base PA
- Adjusting adaptive PA curve
- Slightly increasing flow

### Current Testing

- Increasing nozzle temperature
- Adjusting flow ratio
- Testing reduced fan speeds
Initial calibration data available in:
- Filaments/PETG/Sunlu/

---

## 📊 Included
- Adaptive Pressure Advance testing
- Flow calibration (in progress)

---

## 💡 Notes
This profile is being developed based on real-world testing and structured calibration.

Final values will be added soon.
