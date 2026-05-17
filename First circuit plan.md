# Circuits Assessment 3: Team Division of Labor & Project Tracking

This document outlines the collaborative split, implementation leads, and mathematical verification tasks for **Circuits Assessment 3 (Analog Circuit Design & Simulation)**.

## 📊 High-Level Strategy
* **Pass's Core Focus:** Questions 1, 3, 5, 7, 9 (Signal conditioning, active frequency filtering, multi-input active summing, and mathematical scaling systems).
* **Win's Core Focus:** Questions 2, 4, 6, 8 (Power/precision rectification, non-inverting small-signal amplification, and calculus-based integrator ramp generation).

---

## 🛠️ Task Board & Progress Tracking

### 🧗 Stage 1: Falstad Circuit Simulation & Verification
- [ ] **Q1: Smoothing a Noisy Sensor** (Active LPF, $f_c = 100\text{ Hz}$) — **Lead: Pass**
- [ ] **Q2: AC to Unidirectional Signal** (Passive Bridge Rectifier) — **Lead: Win**
- [ ] **Q3: Producing Smoother DC Output** (Parallel RC Filter, $\Delta V < 0.5\text{ V}$) — **Lead: Pass**
- [ ] **Q4: Amplifying Weak Audio Signal** (Non-Inverting Amp, Gain = $+100$) — **Lead: Win**
- [ ] **Q5: Inverting and Scaling a Signal** (Inverting Amp, Gain = $-10$) — **Lead: Pass**
- [ ] **Q6: Accurate Micro-Signal Rectification** (Active Precision Half-Wave Rectifier) — **Lead: Win**
- [ ] **Q7: Selecting Desired Frequency Range** (Active BPF, $f_0 = 5\text{ kHz}$) — **Lead: Pass**
- [ ] **Q8: Converting Square Wave to Triangle Wave** (Active Integrator with Bleeder $R_f$) — **Lead: Win**
- [ ] **Q9: Shifting and Rescaling Sensor Output** (Inverting Summer + Unity Buffer) — **Lead: Pass**

---

### 📝 Stage 2: Technical Report Drafting & Core Mathematics

#### 🟢 Pass's Deliverables
- [ ] **Draft Q1 Section:** Formalize the geometric mean calculation ($\sqrt{10 \times 1000} = 100\text{ Hz}$) and show steps for selecting $R = 1.59\text{ k}\Omega$ and $C = 1\mu\text{F}$.
- [ ] **Draft Q3 Section:** Document the linear discharge approximation formula to justify the choice of a $100\mu\text{F}$ capacitor to meet the $\Delta V < 0.5\text{ V}$ spec.
- [ ] **Draft Q5 Section:** Derive the standard closed-loop gain expression $A_v = -R_f / R_{in} = -10$.
- [ ] **Draft Q7 Section:** Detail the cascading rules between active high-pass and low-pass stages to establish independent boundary conditions at $5\text{ kHz}$.
- [ ] **Draft Q9 Section:** Provide the system of boundary linear equations ($m=1.25, c=2.5\text{V}$) using the corrected **$+5\text{V}$ positive reference rail** to map all component values ($R_{in}=8\text{k}\Omega, R_{ref}=20\text{k}\Omega$) cleanly.

#### 🔵 Win's Deliverables
- [ ] **Draft Q2 Section:** Formalize the Kirchhoff's Voltage Law (KVL) path during positive/negative half-cycles showing the structural $-1.4\text{V}$ diode drop ($V_{out} = 5\text{V} - 2V_D$).
- [ ] **Draft Q4 Section:** Document the non-inverting gain parameters layout where $1 + R_f / R_1 = 100$.
- [ ] **Draft Q6 Section:** Provide the dual-diode conduction equations to prove how the feedback loop actively compensates for the $0.7\text{V}$ junction threshold down to millivolt scales.
- [ ] **Draft Q8 Section:** Layout the calculus derivation showing how a constant voltage integrates over a half-cycle window ($\Delta V_{out} = -\frac{1}{RC}V_{in}\Delta t$) to hit the targets ($R=1\text{k}\Omega, C=100\text{nF}$).

---

### 🏁 Stage 3: Quality Control & Final Integration
- [ ] **Cross-Review Code Links:** Pass to verify Win's Falstad textual array setups for export safety; Win to audit Pass's multi-stage op-amp nodal currents.
- [ ] **Academic Integrity Alignment:** Both partners independently write and personalize their *Performance Discussion & Reflection* subsections (Part G) for every question to ensure individual unique wording prior to submission compilation.
