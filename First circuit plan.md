# SYS-208:00010 Assessment Task Tracking & Labor Division

This project board tracks implementation, derivations, and peer verification for the foundational DC circuit analysis and technology comparison problem set.

## 📋 General Submission Guidelines (Strictly Enforced)
Every question item must explicitly include the following blocks in the final compilation to receive full credit:
- [ ] **State Knowns:** List all numerical and component parameters cleanly with matching metric units.
- [ ] **Circuit Visuals:** Include an annotated schematic sketch showing node tags, calculated current arrows ($I$), and polarity signs ($+/-$).
- [ ] **Equation Setup:** State formulas in parametric form *before* entering numerical numbers.
- [ ] **Step-by-Step Logic:** Show intermediate arithmetic progression cleanly.
- [ ] **Closing Summary:** Write out the final resolution in full, grammatically complete sentences.

---

## 🛠️ Individual Question Assignments & Sub-Task Boards

### 🟢 Pass's Technical Focus Areas: Questions 1, 3, and 5

#### 🟦 Question 1: Single-Resistor Core Verification & Consistency
- [ ] **Task 1.1:** Calculate the exact value of the unknown resistor using Ohm's Law given $V = 5.00\text{ V}$ and $I = 1.064\text{ mA}$.
- [ ] **Task 1.2:** Calculate the necessary source voltage ($V_s$) fueling the loop network.
- [ ] **Task 1.3:** Perform a physical consistency audit to prove whether the combination of ideal meters matches loop boundary conditions.

#### 🟦 Question 3: Parallel Networks & Diagnostic Instrument Troubleshooting
- [ ] **Task 3.1:** Calculate total equivalent resistance ($R_{eq}$) for the parallel stack ($2.2\text{ k}\Omega \parallel 4.7\text{ k}\Omega \parallel 10\text{ k}\Omega$).
- [ ] **Task 3.2:** Compute the total current ($I_{total}$) entering the split terminal cluster from a $5.0\text{ V}$ source.
- [ ] **Task 3.3:** Calculate individual branching current levels running through $R_1$, $R_2$, and $R_3$.
- [ ] **Task 3.4:** Mathematically prove exactly where an ammeter was spliced inside the physical circuit trace to read $2.27\text{ mA}$.
- [ ] **Task 3.5:** Specify the structural nodes where a voltmeter reading $5.0\text{ V}$ must be probing.
- [ ] **Task 3.6:** Draft a short technical explanation outlining why that specific voltage reading can occur at multiple locations in a parallel topology.

#### 🟦 Question 5: Multi-Source Bridge Network Nodal Analysis
- [ ] **Task 5.1:** Set up the Kirchhoff's Current Law (KCL) node equation modeling currents converging at node $V_x$.
- [ ] **Task 5.2:** Algebraically isolate and solve for the exact steady-state potential of node $V_x$.
- [ ] **Task 5.3:** Calculate the directional branching currents flowing cleanly through $R_2$, $R_3$, and $R_4$.
- [ ] **Task 5.4:** Perform a comprehensive Kirchhoff's Voltage Law (KVL) loop calculation to verify the nodal results.
- [ ] **Task 5.5:** Contrast the source inputs ($V_1 = 5.0\text{ V}$ vs. $V_2 = 3.0\text{ V}$) to state which power source exerts greater mathematical influence over $V_x$.
- [ ] **Task 5.6:** Formulate a parametric proof outlining how increasing the scale of load resistor $R_2$ alters the value of $V_x$.

---

### 🔵 Win's Technical Focus Areas: Questions 2, 4, and 6

#### 📙 Question 2: Series-Parallel Indeterminacy Resolution
- [ ] **Task 2.1:** Evaluate the total circuit resistance ($R_{total}$) using a $1.00\text{ V}$ source driving a $1.667\text{ mA}$ active current loop.
- [ ] **Task 2.2:** Determine the precise resistance of $R_2$ based on the given localized voltage drop ($333.3\text{ mV}$).
- [ ] **Task 2.3:** Isolate and solve for the combined residual value of the series elements ($R_1 + R_3$).
- [ ] **Task 2.4:** Draft a network topology proof explaining why $R_1$ and $R_3$ cannot be extracted individually from the current measurement loop layout.
- [ ] **Task 2.5:** Detail one specific layout adjustment or secondary hardware measurement probe location required to solve all distinct values.

#### 📙 Question 4: NTC Thermistor Voltage Divider Instrumentation
- [ ] **Task 4.1:** Algebraically derive the full transfer function expression for $V_{out}$ as a function of $V_{in}$, $R_s$, and $R_T$.
- [ ] **Task 4.2:** Compute $V_{out}$ under equalized balance conditions where $R_s = R_T = 10\text{ k}\Omega$.
- [ ] **Task 4.3:** Reverse-engineer and calculate the exact resistance of thermistor $R_T$ when the output voltage shifts to $3.0\text{ V}$.
- [ ] **Task 4.4:** Document the material physics governing how an Negative Temperature Coefficient (NTC) thermistor's bulk resistance changes when ambient heat rises.
- [ ] **Task 4.5:** Map out how the resulting $V_{out}$ potential moves across the ADC rail when temperatures scale up.
- [ ] **Task 4.6:** Explain how this specific hardware division profile allows a standard digital microcontroller to infer real-world temperature.
- [ ] **Task 4.7:** Evaluate why a voltage divider setup is uniquely optimized for processing passive resistive transducer sensors.

#### 📙 Question 6: Thevenin & Norton Network Equivalents
- [ ] **Task 6.1:** Temporarily desolder $R_2$ from the network to calculate the open-circuit Thevenin Voltage ($V_{th}$).
- [ ] **Task 6.2:** Zero out both active DC power supplies ($V_1, V_2 \rightarrow 0$) to calculate the lookup equivalent Thevenin Resistance ($R_{th}$).
- [ ] **Task 6.3:** Reconnect the $R_2$ load element onto your simplified network model to calculate the current and voltage drops.
- [ ] **Task 6.4:** Determine the short-circuit Norton Current ($I_N$) for this network topology.
- [ ] **Task 6.5:** Graphically/mathematically verify that Norton resistance ($R_N$) equates to $R_{th}$.
- [ ] **Task 6.6:** Construct an executive analysis explaining why Thevenin and Norton reduction models are useful when modeling sensor conditioning interfaces.

---

### 🤝 Collaborative / Split Essay Deliverable

#### 👥 Question 7: CMOS vs. Bipolar Core Architectural Assessment
- [ ] **Pass's Core Focus:** Compare CMOS and Bipolar structures in terms of baseline **power consumption profiles** (static vs. dynamic) and **digital logic integration density** scaling. Provide 2 standard industry CMOS application examples.
- [ ] **Win's Core Focus:** Compare CMOS and Bipolar configurations regarding **analog matching accuracy/linearity** and thermal noise floor performance characteristics. Provide 2 standard industry Bipolar hardware application examples.
- [ ] **Final Alignment Check:** Review combined paragraphs together to ensure smooth conceptual flow and zero repetitive formatting overlap before publishing.
