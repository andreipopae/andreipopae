# Andrei-Emanuel Popa

**Applied Electronics Graduate | Data Analysis · Process Improvement · Testing · Reliability
Bucharest, Romania · [andreipopae@gmail.com](mailto:andreipopae@gmail.com) · LinkedIn: www.linkedin.com/in/andrei-emanuel-59149635b

---

Final-year Applied Electronics student at **Politehnica Bucharest (ETTI)**, graduating June 2026.
I work at the boundary between theory and the bench: analog and power-electronics design, closed-loop
control, and reliability/quality methods. I like problems where the answer has to survive contact with
real hardware, not just a simulator.

**Core areas:** bench measurement · acceptance sampling & reliability analysis · power electronics & control · analog circuit design
**Tools:** SPICE · PSIM · OrCAD / Altium · Python · C++ · Excel · oscilloscope / function generator / power supply / multimeter

---

## Projects

### 1. Reliability & Quality Engineering — Acceptance Sampling & Failure Analysis
> *Statistical quality control and reliability characterization of electronic components.*

**Overview.** A full reliability-and-quality study: building inspection plans for incoming lots and
characterizing component life from test data.

**What I did**
- Built **single, double and multiple acceptance-sampling plans** per **MIL-STD-105E (ANSI/ASQC Z1.4, ISO 2859)** for AQL levels 0.15 / 0.65 / 2.5 / 10 %, inspection level II, and compared **normal vs. tightened** severity.
- Classified defects (critical / major / minor A & B) and reasoned about lot accept/reject decisions and switching rules.
- Computed **reliability indicators** — F(t), R(t), failure density f(t), and failure rate z(t) — from a life test on **1000 transistors** measured every 100 h; plotted the reliability and hazard curves and extracted quantiles.
- Analyzed a **truncated test** on 200 transistors and derived F, R, hazard and quantile estimates.
- Identified the **failure-time distribution** (exponential / Weibull / normal) using probability paper and **concordance tests** (Kolmogorov–Smirnov, Koziol–Byar) across several risk levels — best fit: Weibull.

**Tools:** Excel · MIL-STD-105E tables · reliability software · sqconline calculator
**What it demonstrates:** AQL sampling, OC/ASN curves, reliability metrics, hazard-rate (bathtub) reasoning, distribution fitting — the everyday toolkit of a reliability/quality engineer.

📎 [Repository →](https://github.com/andreipopae/reliability-quality-engineering)

---

### 2. PWM Current Control — One-Quadrant DC-DC Converter
> *Closed-loop current regulator design, tuning and stability verification.*

**Overview.** Design and validation of a current-control loop for a one-quadrant DC-DC converter
driving an RL load, optimized for step response.

**What I did**
- Derived the **transfer functions** of converter + load, current transducer and PWM modulator; linearized the (non-linear) converter around its operating point using averaged state variables.
- Designed and **tuned a PI controller via the modulus-optimum criterion**, and sized the real component values (R0, R1, C1) and the measurement filter.
- Ran **transient simulation in PSIM**: step response with settling time and overshoot compared against theory (≈4.72·Tσ, 4.3 %), duty cycle, current ripple (measured vs. calculated) and error.
- **Robustness tests:** ±25 % / ±50 % supply variation, ±50 % load step, and a trapezoidal reference (steady-state error for a ramp input).
- **Stability:** AC sweep → Bode plot → measured **phase margin ≈ 70°** ⇒ stable loop.

**Tools:** PSIM · control theory · power electronics
**What it demonstrates:** closed-loop control design, power-electronics modeling, frequency-domain stability analysis, simulation-driven validation against theoretical targets.

📎 [Repository →](https://github.com/andreipopae/pwm-current-control-converter)

---

### 3. Voltage-Controlled Audio Preamplifier — Analog Design & Hardware Build
> *Discrete-BJT analog design taken from schematic to a working board.*

**Overview.** A voltage-controlled audio preamplifier (gain 1–30) with Baxandall tone control,
designed, hand-analyzed, simulated **and physically built**. Developed in the ETTI–Infineon Romania program.

**What I did**
- Designed a **3-stage discrete-BJT** preamplifier (common-emitter stages) with a ±13 dB Baxandall tone control, single 13 V supply, 800 Ω load, 30 mV / 3 kHz input.
- **Hand-calculated the DC operating points** for every transistor and verified each stays in the active region and within safe-operating limits (Vce < 65 V, Ic < 100 mA for the BC546B).
- Produced the **BOM** and a perfboard layout (DIYLC) and **assembled the board in THT**.
- Validated behaviour against **SPICE** simulation (waveforms and operating points for Vc = 0 V and 3 V).

**Tools:** SPICE · DIYLC · hand analysis · THT assembly / soldering
**What it demonstrates:** analog circuit design, biasing and safe-operating-area analysis, BOM/DFM basics, and the hands-on bench skill of getting a real board to behave.

📎 [Repository →](https://github.com/andreipopae/analog-audio-preamplifier)

---

### 4. Bachelor Thesis — Edwards vs. Montgomery Elliptic Curves (Ed25519 vs. X25519)
> *Comparative performance analysis of two elliptic-curve schemes on a common field.*

**What I did**
- Compared **Ed25519** (Edwards curve, digital signatures) and **X25519** (Montgomery curve, key exchange) on the shared Curve25519 field.
- **Benchmarked** signing, verification and key-exchange performance in **Python** and documented the methodology and results; figures in matplotlib, written and typeset in **LaTeX**.

**Tools:** Python · matplotlib · LaTeX
**What it demonstrates:** applied-cryptography understanding, structured benchmarking methodology, and technical writing.

📎 [Repository →](https://github.com/andreipopae/thesis-ed25519-vs-x25519)

---

## Experience

**Robotics & Coding Instructor (Part-time)** — Future Minds, Bucharest · *Sep 2024 – Jun 2026*
Hands-on robotics workshops (hardware assembly, logic-circuit debugging), kit maintenance for reliable
sessions, and teaching block-based coding — plus a lot of practice explaining technical ideas clearly.

## Education

**B.Eng. Applied Electronics** — Politehnica Bucharest (ETTI) · *2022 – 2026*
Relevant coursework: Reliability & Quality Engineering · Power Electronics & Control Systems ·
Fundamental Electronic Circuits · PCB Design.

---

*Open to test / validation / reliability / quality engineering internships and graduate roles in Bucharest.*
