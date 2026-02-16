
# labscalecoolingtower

> To design, manufacture, and validate a transparent, lab-scale cooling tower to demonstrate evaporative cooling principles and heat transfer phenomena for educational purposes.

---

## Executive Summary

This project focuses on the design and realization of a **Lab-Scale Cooling Tower** as part of an integrated HVAC educational system. The primary goal was to create a functional, transparent unit that visualizes evaporative cooling phenomena while achieving measurable thermal performance.

**Key Results:**
* **Cooling Range:** 6°C (Target: ≥5°C)
* **Approach Temperature:** 2.41°C
* **Effectiveness:** ~60.8%
* **Water/Air Ratio (L/G):** 1.03
* **Evaporation Loss:** 0.151 kg/hour (Indicating high efficiency)

---

## Project Objectives & Requirements

### The Problem (Design Gap)
Industrial cooling towers are typically opaque, massive, and permanent structures. This makes them unsuitable for explaining fluid dynamics and internal heat transfer mechanisms to students effectively.

### The Solution
A portable, table-top **Induced Draft Counter-Flow Cooling Tower** featuring a fully transparent acrylic casing to allow direct observation of the water distribution and fill wetting processes.

---

## Engineering Specifications

| Category | Parameter | Target Spec / Design Value |
| :--- | :--- | :--- |
| **Structure** | Material | Transparent Acrylic (Clear) |
| | Dimensions | Compact / Lab Scale (40x40 cm) |
| **Fill Media** | Type | Honeycomb / PVC Film Fill (2 units) |
| **Air System** | Fan Type | Axial Fan (Induced Draft) |
| | Fan Diameter | 10 inch |
| | Air Flow Rate | ≈ 0.00468 kg/s |
| **Water System** | Pump Type | Submersible Pump |
| | Power | 10-20 Watt |
| | Water Flow Rate | ≈ 0.00483 kg/s |
| **Performance** | Cooling Capacity | ≈ 0.076 kW (76 Watts) |
| | Target Range | ≥ 5°C (Actual: 6°C) |
| | Target Approach | ≤ 4°C (Actual: 2.41°C) |

---

## Detailed Design & Components

### 1. Conceptual Design Choice
The team selected the **Induced Draft (Top Fan)** configuration over Forced Draft.



* **Reasoning:** This configuration provides better airflow distribution across the filler, reduces the risk of hot air recirculation, and leaves the main body unobstructed for better visualization.
* **Fill Type:** **Film Fill (Honeycomb)** was chosen for its higher specific surface area per volume compared to splash fill, which is crucial for a compact unit.



### 2. Bill of Materials (Key Items)
* **Body:** Custom Clear Acrylic (~9842 cm² total area).
* **Active Components:**
    * 1x Axial Fan (10 inch).
    * 1x Submersible Pump (Rosston SP2600, 20W).
* **Piping:** 1-inch PVC pipes, Elbows, T-connectors, and a 1/2 inch Ball Valve for drainage.
* **Fill:** 2x Honeycomb/PVC Filler blocks (225mm x 200mm).

### 3. Fabrication Process
* **Acrylic Fabrication:** Laser cutting and assembly using specialized acrylic adhesive to ensure water-tight seals.
* **Assembly:** Mounting the fill media, securing the fan to the top plate using cable ties, and positioning the submersible pump in the basin.
* **Piping Integration:** Connecting the pump to the top distribution nozzle using PVC piping and installing the drain valve.

---

## Engineering Analysis & Results

### Thermal & Fluid Data
The system analysis focused on the interaction between water and air within the filler media.



| Parameter | Value | Notes |
| :--- | :--- | :--- |
| **Inlet Water Temp** | 32°C | |
| **Cooling Range** | 6°C | Target was ≥5°C |
| **Approach** | 2.41°C | Target was ≤4°C |
| **Effectiveness ($\epsilon$)** | 60.8% | |
| **L/G Ratio** | 1.03 | Indicates balanced flow |
| **Total Heat Rejected** | ~121 W | Measured at Condenser side |

### Testing & Validation

**Methodology**
Validation involved verifying mechanical functionality and thermal efficiency using smart probe thermometers (Testo 115i), thermocouples, and wattmeters.

**Functional Testing & Issues**
* **Circulation:** The submersible pump successfully circulated water against the designed head height.
* **Airflow:** The 20-watt fan successfully overcame the system pressure drop (40 Pa).
* **Defect Identified:** Initial tests revealed leakage where water missed the filler media due to imprecise holder positioning.
* **Iteration:** The Filler Holder position was modified, resulting in even distribution and zero leakage.

**Thermal Validation Results (Condenser Side)**
The cooling tower's effectiveness was validated by its ability to reject heat from the integrated refrigeration system.
* **Temperature Discharge (Gas):** 56.3°C.
* **Temperature Liquid:** 31.1°C.
* **Delta T:** A temperature drop of approximately **25.2 K** was achieved in the refrigerant line, confirming effective condensation.

---

## Final Prototype Features

The final assembly resulted in a robust, portable unit meeting all educational requirements.
* **Full Transparency:** Clear acrylic casing provides 100% visibility of internal components.
* **Integrated Piping:** Neat PVC piping connects the basin to the top nozzle, including a dedicated drain valve.
* **Stability:** The structure is stable and compact, suitable for laboratory tabletops.

---

## Discussion & Conclusion

### Success Factors
* **Mechanical Integrity:** Continuous operation without overheating; low total power consumption (~40 Watts).
* **Visual Education:** Successfully allows observation of flow phenomena (e.g., channeling, wetting) impossible to see in industrial units.
* **Performance:** Exceeded minimum Cooling Range target (Actual: 6°C vs Target: 5°C).

### Lessons Learned
* **Precision is Critical:** Small deviations in water distribution assembly can cause channeling, significantly reducing thermal efficiency.
* **Flow Balance:** Maintaining the L/G ratio near 1.0 is crucial; a fan that is too strong causes drift loss, while a weak fan results in insufficient cooling.

### Recommendations
* **Variable Media:** Test different fill types (Splash vs. Film) to experimentally compare efficiency.
* **Data Automation:** Integrate Arduino/ESP32 sensors for real-time data logging to reduce manual reading errors.

## Pictures and Diagrams

The following visual assets document the design and realization process of the cooling tower.

<img width="308" height="367" alt="image" src="https://github.com/user-attachments/assets/025b0638-d005-4969-a7e5-dbfc0dd4fb91" />
<img width="940" height="664" alt="image" src="https://github.com/user-attachments/assets/35ccf3f3-f4b5-4c0c-b1b5-120c70b6e4ac" />
<img width="474" height="633" alt="image" src="https://github.com/user-attachments/assets/52e6956e-602f-4a18-bbec-c86bb2a1c683" />
<img width="355" height="633" alt="image" src="https://github.com/user-attachments/assets/9a505287-e866-47cd-9188-fbb5aec6ddeb" />


