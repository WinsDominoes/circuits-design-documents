# SYS-208 Project Plan: Temperature-Controlled Fan System for Server Rack

**Study Group:** Pass & Win  
**Platform:** Tinkercad (Simulation-Based)

---

## 1. Project Overview
This project involves designing an automated cooling system that adjusts fan speed based on ambient temperature using an Arduino, a TMP36 sensor, and a potentiometer for manual threshold adjustment.

## 2. Work Split & Responsibilities

| Section | Lead | Focus for Individual Report |
| :--- | :--- | :--- |
| **1. Problem Definition** | **Joint** | Define the context (e.g., cooling for electronics)[cite: 1]. |
| **2. Design Objectives** | **Joint** | Set specific performance goals and constraints[cite: 1]. |
| **3. Platform Justification** | **Joint** | Explain why Tinkercad was used for remote work[cite: 1]. |
| **4. System Block Diagram** | **Pass** | High-level signal flow from sensing to actuation[cite: 1]. |
| **5. Circuit Design** | **Win** | Interface design between MCU and components[cite: 1]. |
| **6. Pin Assignment** | **Win** | Technical mapping of I/O pins and PWM selection[cite: 1]. |
| **7. ADC & Sensor Analysis** | **Pass** | **Heavy Math**: Voltage mapping and ADC calculations[cite: 1]. |
| **8. Control Algorithm** | **Win** | **Heavy Logic**: Flowchart and pseudocode logic[cite: 1]. |
| **9. Testing & Validation** | **Pass** | Comparison of math predictions vs. actual results[cite: 1]. |
| **10. Optimization** | **Win** | Software features (Hysteresis and PWM control)[cite: 1]. |
| **11. Reflection** | **Both** | Individual lessons learned and future upgrades[cite: 1]. |

---

## 3. Technical Specifications

### Mathematical Modeling (Pass)
To be used for Section 7 and 9 of the report:
*   **Sensor Formula:** $$V_{out} = (10\text{mV} \times T_{Celsius}) + 500\text{mV}$$[cite: 1]
*   **ADC Resolution:** $$1 \text{ unit} = \frac{5V}{1024} \approx 4.88\text{mV}$$[cite: 1]
*   **Target Calculation:** At $30^{\circ}C$, expected $V_{out} = 0.8V$, resulting in a digital value of $\approx 164$[cite: 1].

### Logic & Optimization (Win)
To be used for Section 8 and 10 of the report:
*   **Hysteresis:** Implement a 2-degree "buffer" to prevent the fan from flickering at the threshold[cite: 1].
*   **PWM Control:** Use `analogWrite()` to scale fan speed dynamically between $30^{\circ}C$ and $45^{\circ}C$[cite: 1].

---

## 4. Implementation Evidence Checklist (Part A)
*Required for submission[cite: 1]:*
- [ ] Shared Tinkercad project link.
- [ ] High-resolution screenshot of the full circuit.
- [ ] Screenshots of Serial Monitor showing digital temperature readings.
- [ ] Demonstration video showing the fan turning on/off as temperature changes.
- [ ] Final Arduino source code (`.ino`).

---

## 5. Important Reminders
*   **Individual Work:** While we share the circuit and data, the report text, flowcharts, and analysis must be written independently[cite: 1].
*   **Mandatory Requirements:** The system must use at least 2 analog sensors (TMP36 + Potentiometer) and 1 actuator (DC Motor)[cite: 1].
