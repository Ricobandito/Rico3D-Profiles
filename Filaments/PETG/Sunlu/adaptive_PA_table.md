# Adaptive Pressure Advance – SUNLU PETG

Printer: Snapmaker U1  
Slicer: OrcaSlicer  
Material: SUNLU PETG  

---

## Test Setup

PA range: 0.00 – 0.05  
Step: 0.005  

Speeds tested:
- 50 mm/s
- 100 mm/s
- 150 mm/s
- 200 mm/s
- 250 mm/s

Accelerations tested:
- 1000 mm/s²
- 2000 mm/s²
- 4000 mm/s²

---

## Adaptive PA Development History

### v0.1 – Initial PA Pattern Interpretation

First adaptive PA table based on early PA pattern interpretation.

This version included extrapolated flow values up to 18.7 mm³/s based on the PA pattern interpretation.  
The actual filament profile was never intended to exceed 14.5 mm³/s max volumetric speed, so later versions focus only on the relevant flow range up to 14.5 mm³/s.

### v0.2 – Expanded Low-Flow Table

Added more low-flow points after further speed and profile adjustments.

This version provided better control in the lower volumetric flow range and improved the transition between low, mid and high flow regions.

### v0.3 – Compatibility Test

Current test version adjusted for broader material compatibility, especially:

- PETG as support/interface material for PLA
- PLA as support/interface material for PETG
- PETG-to-PETG support compatibility

Low- to mid-flow PA values were slightly reduced to improve bonding and reduce potential under-extrusion in sensitive areas.

---

## Current Adaptive PA Table – v0.3 Compatibility Test

```text
0.017,2.0,1000
0.019,2.5,1000
0.020,3.0,1000
0.021,3.7,1000
0.022,5.5,1000
0.023,7.4,1000
0.025,9.3,1000
0.026,11.1,1000
0.027,14.5,1000

0.018,2.0,2000
0.020,2.5,2000
0.021,3.0,2000
0.022,3.7,2000
0.023,5.5,2000
0.024,7.4,2000
0.026,9.3,2000
0.027,11.1,2000
0.028,14.5,2000

0.020,2.0,4000
0.022,2.5,4000
0.023,3.0,4000
0.024,3.7,4000
0.025,5.5,4000
0.026,7.4,4000
0.028,9.3,4000
0.029,11.1,4000
0.030,14.5,4000
