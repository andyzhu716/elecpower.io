---
title: "Busbar Sizing and Selection: Engineer's Complete Handbook"
description: "Step-by-step busbar sizing methodology for electrical engineers. Covers ampacity calculation, short-circuit withstand verification, temperature derating, and voltage drop analysis with worked examples."
date: 2026-04-09
lastmod: 2026-04-09
draft: false
tags:
  - busbar sizing
  - busbar calculation
  - ampacity
  - short-circuit
  - electrical engineering
  - busbar selection
  - current rating
categories:
  - Technical Guide
  - Engineering Handbook
featured_image: "images/blog/busbar-sizing-selection-engineers-handbook.jpg"
---

Selecting and sizing a busbar system requires matching electrical, mechanical, and environmental parameters to a specific installation. Get it wrong and the system either runs hot — shortening insulation life and creating fire risk — or costs far more than necessary through over-specification. Get it right and the busbar performs reliably for decades with minimal maintenance.

This handbook gives electrical engineers and specifiers a rigorous, step-by-step methodology for correctly sizing busbar systems across all voltage and current classes. It covers the three mandatory checks — ampacity, short-circuit withstand, and voltage drop — and explains the environmental and application variables that modify each calculation.

**Key Takeaways:**
- Busbar sizing requires three simultaneous checks: ampacity, short-circuit withstand, and voltage drop — all three must pass
- The most common sizing error is neglecting ambient temperature and altitude derating, leading to chronic overheating in service
- Short-circuit verification must use the **available fault current at the bus location**, not the bus's rated fault capacity
- Voltage drop is frequently overlooked but can exceed limits in long runs, particularly at low voltages or high load power factors
- Always apply a minimum 25% margin between calculated load current and the bus's continuous current rating

---

## Table of Contents

1. [Sizing Fundamentals: The Three Mandatory Checks](#1-sizing-fundamentals-the-three-mandatory-checks)
2. [Ampacity Calculation](#2-ampacity-calculation)
3. [Short-Circuit Withstand Verification](#3-short-circuit-withstand-verification)
4. [Voltage Drop Analysis](#4-voltage-drop-analysis)
5. [Environmental Derating Factors](#5-environmental-derating-factors)
6. [Busbar Material and Profile Selection](#6-busbar-material-and-profile-selection)
7. [Selection Checklist and Worked Example](#7-selection-checklist-and-worked-example)
8. [Frequently Asked Questions](#8-frequently-asked-questions)

---

## 1. Sizing Fundamentals: The Three Mandatory Checks

Every busbar sizing exercise must satisfy three independent criteria simultaneously. A busbar that passes one or two checks but fails the third is not adequately sized.

### Check 1: Continuous Ampacity

The busbar must carry the maximum expected continuous load current without exceeding its rated temperature limit. This is the most fundamental check and the one most frequently performed. However, it is also the one most commonly misapplied — ampacity ratings published in catalogues are always specified under defined test conditions (typically 30°C or 40°C ambient, sea level, natural convection, sinusoidal current). Real installations rarely match these conditions exactly, so **derating is almost always required**.

### Check 2: Short-Circuit Withstand

The busbar must survive the mechanical and thermal stresses of a short-circuit current without permanent damage. The mechanical stress from electromagnetic forces during a fault is proportional to the **square of the instantaneous fault current** — a 200kA RMS fault produces electromagnetic forces of several thousand newtons per meter on the conductor assembly. The busbar's short-circuit rating must exceed the maximum available fault current at its point of installation.

### Check 3: Voltage Drop

The busbar must limit voltage drop to acceptable levels under full-load conditions. While voltage drop does not damage the busbar itself, excessive voltage drop degrades connected equipment performance (motors run hot, electronics malfunction, protective devices may not operate correctly at defined pickup voltages). Voltage drop limits are typically specified by the client or by relevant standards; common limits are 2–3% for main feeders and 3–5% for branch circuits.

### The Sizing Sequence

Perform the three checks in the following order — they are independent but sequential in practice:

```
Step 1 → Determine design current (load analysis)
Step 2 → Select tentative busbar rating from manufacturer catalogue
Step 3 → Apply environmental derating to confirm the selected bus meets ampacity
Step 4 → Verify short-circuit withstand against available fault current at installation location
Step 5 → Calculate voltage drop at full load — if it exceeds limit, increase busbar size
Step 6 → Confirm mechanical dimensions are compatible with installation space
```

> **Related reading:** [How to Choose the Right Busbar System for a Power Plant](./how-to-choose-the-right-busbar-system-for-a-power-plant.md) covers the qualitative selection between IPB, NSPB, SPB, and cast resin busway. This handbook covers the quantitative sizing methodology for whichever type is selected.

---

## 2. Ampacity Calculation

### 2.1 Design Current

The starting point for ampacity sizing is the maximum expected continuous load current. This must be established from the load study for the installation:

```
I_design = I_max × (1 + G) × D
```

Where:
- `I_max` = maximum continuous load current under worst-case operating conditions (A)
- `G` = growth margin factor (decimal; typically 0.10 to 0.25 for a 10–25% future load growth allowance)
- `D` = diversity factor (decimal; accounts for the fact that not all loads operate simultaneously; typically 0.8 to 1.0 for a well-loaded main bus)

**Practical rule:** Specify a busbar with a continuous current rating of at least **125% of the calculated design current**. This provides a built-in margin for measurement uncertainty, temporary overloads, and moderate future load growth without requiring a re-specification.

### 2.2 Busbar Ampacity Ratings

Busbar ampacity depends on three factors: conductor cross-section, conductor material, and cooling conditions. Published ampacity tables from manufacturers provide ratings under standard reference conditions. These must be corrected for actual installation conditions.

**Standard reference conditions** (per IEEE C37.23 and IEC 61439):
- Ambient temperature: 30°C (NEMA) or 40°C (IEC)
- Altitude: ≤ 1,000m
- Installation: Indoors, natural convection cooling
- Load current: Pure sinusoidal, 50/60Hz
- No solar heating contribution
- Installation with minimum specified clearances

**Approximate ampacity ranges for common busbar configurations:**

| Configuration | Material | Typical Current Range (per phase) |
|--------------|----------|----------------------------------|
| IPB (large generator) | Aluminum | 3,000A – 30,000A+ |
| IPB (ultra-high current) | Aluminum/Copper | 30,000A – 50,000A+ |
| NSPB | Aluminum | 1,000A – 6,300A |
| SPB | Aluminum | 1,000A – 15,000A |
| Cast resin busway | Aluminum/Copper | 250A – 6,300A |
| Low-voltage enclosed busbar | Copper | 100A – 6,300A |

### 2.3 Step-by-Step Ampacity Sizing

**Step 1:** Calculate design current using the formula above.

**Step 2:** Identify the busbar configuration appropriate for the application (IPB for generator connections above ~3,000A; NSPB/SPB for medium-voltage distribution; cast resin for harsh environments or low-voltage distribution).

**Step 3:** Select a tentative busbar rating from a manufacturer's catalogue. The selected rating must exceed the design current multiplied by the relevant environmental derating factor (see Section 5):

```
I_rated_required = I_design / (K_total)
```

Where `K_total` is the product of all applicable derating factors. If no derating applies (indoor, sea level, moderate ambient), `K_total = 1.0`.

**Step 4:** Verify that the selected busbar's continuous current rating meets this requirement. If not, select the next larger rating.

### 2.4 Temperature Rise and Heat Dissipation

The temperature rise of a busbar under load is determined by the balance between heat generated and heat dissipated:

```
Heat Generated = I² × R × t (watts)
Heat Dissipated = h × A × ΔT (watts)
```

At equilibrium (steady state): `I² × R = h × A × ΔT`

Where:
- `I` = load current (A)
- `R` = conductor AC resistance (Ω/m)
- `h` = heat transfer coefficient (W/m²·K) — depends on natural or forced convection, enclosure type
- `A` = effective surface area for heat dissipation (m²/m)
- `ΔT` = temperature rise above ambient (K)

For a given busbar geometry and material, temperature rise is proportional to the **square of the current**. Doubling the current produces four times the heat generation and approximately four times the temperature rise if散热 is purely conductive. In practice, the relationship is slightly less than squared due to increased convective cooling at higher temperatures.

**Maximum permissible operating temperature:** Busbar systems are typically rated for a maximum conductor temperature of 85°C (105°C for high-temperature designs). At an ambient of 40°C, this permits a maximum temperature rise of 45K. The conductor temperature limit exists to protect insulation materials, connections, and surrounding equipment from thermal degradation.

---

## 3. Short-Circuit Withstand Verification

### 3.1 Why Short-Circuit Verification Is Mandatory

When a short-circuit occurs, the instantaneous electromagnetic force on a busbar conductor can reach thousands of newtons per meter. A busbar inadequately rated for short-circuit withstand may:

- Permanently deform conductors (plastic deformation beyond elastic limit)
- Damage or crack insulator supports
- Distort enclosure geometry, compromising phase clearances
- Create Phase-to-phase or phase-to-ground fault paths, transforming a minor fault into a major incident

### 3.2 Short-Circuit Parameters

The relevant short-circuit parameters for busbar sizing are:

**Short-time withstand current (Icw):** The RMS value of symmetrical short-circuit current the busbar can carry for the specified duration (typically 1s or 3s) without suffering damage. Expressed in kA RMS.

**Peak withstand current (Ipk):** The maximum instantaneous peak current the busbar can withstand without mechanical failure. Expressed in kA peak. For 50/60Hz systems, `Ipk ≈ 2.55 × Icw` for a fully asymmetric fault at maximum DC offset.

**Mechanical force calculation:**

```
F = (μ₀ / 2π) × (I₁ × I₂ / d) × L
```

For three-phase faults on parallel conductors:

```
F_peak = 0.2 × (Ipk² / d) × L   [in newtons, for flat bus bars on edge]
```

Where:
- `Ipk` = peak instantaneous fault current (A)
- `d` = center-to-center distance between phase conductors (m)
- `L` = span length between support insulators (m)

**This equation shows that electromagnetic force is proportional to the square of the fault current and the span length, and inversely proportional to conductor spacing.** Long spans and high fault currents create the most severe mechanical loading.

### 3.3 Verification Procedure

**Step 1:** Determine the maximum available short-circuit current at the busbar installation location. This requires a short-circuit study of the power system, typically performed by the project's electrical engineer using software (ETAP, PowerFactory, PSCAD) or hand calculations following IEC 60909 or ANSI/IEEE C37.010.

**Step 2:** Determine the maximum duration of the fault current, which is controlled by the upstream protective device (circuit breaker or fuse) clearing time. Standard durations for busbar short-circuit ratings are 1s and 3s. Confirm the protective device coordination ensures the fault is cleared within the busbar's rated duration.

**Step 3:** Verify both conditions:

```
Icw (rated) ≥ I_available_RMS
Ipk (rated) ≥ Ipk_available = 2.55 × I_available_RMS (for fully asymmetric 50/60Hz fault)
```

If the available fault current exceeds the busbar's standard short-circuit rating, the options are:
1. Select a higher-rated busbar (higher Icw/Ipk)
2. Add series reactance to limit fault current (increases impedance and voltage drop — use carefully)
3. Modify the upstream system to reduce available fault current

### 3.4 Short-Circuit Ratings by Application

| Application | Typical Available Fault Level | Standard Icw Rating |
|-------------|------------------------------|---------------------|
| Auxiliary distribution | 25–40kA RMS | 40kA / 1s or 3s |
| Medium-voltage unit connections | 40–80kA RMS | 63–80kA / 3s |
| Large generator connections | 80–160kA RMS | 100–200kA / 3s |
| Ultra-large generator (1,000MW+) | 160–300kA RMS | 200–300kA / 3s |
| EHV station connections | Up to 100kA RMS | 100–130kA / 3s |

---

## 4. Voltage Drop Analysis

### 4.1 Why Voltage Drop Matters

Excessive voltage drop in a busbar run has practical consequences that extend beyond simple voltage reduction:

- Motors drawing high current at reduced voltage draw higher current and run hot. A 5% voltage drop at full load can increase motor current by 5–7%, significantly reducing motor life.
- Lighting loads (especially discharge lamps and LEDs) produce noticeably reduced output at voltages below rated.
- Protective relays and circuit breakers are calibrated at system voltage. At significantly reduced voltage, protective devices may fail to operate correctly or may not clear faults.
- In systems with long runs between the source transformer and the load, voltage drop can result in the load never receiving full rated voltage, even at no load.

### 4.2 Voltage Drop Formula

For a three-phase AC busbar:

```
Vd = √3 × I_load × (R cos φ + X sin φ) × L / 1000   [in volts]
```

Where:
- `I_load` = load current (A)
- `R` = AC resistance per conductor per unit length (mΩ/m)
- `X` = reactance per conductor per unit length (mΩ/m)
- `L` = one-way length of the busbar run (m)
- `φ` = load power factor angle
- `cos φ` = load power factor

**Simplified formula (using impedance magnitude):**

```
Vd = √3 × I_load × Z × L / 1000   [in volts]
```

Where `Z = √(R² + X²)` is the impedance per conductor per unit length (mΩ/m).

For low-voltage runs (below 1,000V) or long runs, the simplified formula may underestimate voltage drop if power factor is low, because reactive voltage drop (I×X×L×sin φ) is significant at low power factors. Always use the full formula for power factors below 0.8.

### 4.3 Voltage Drop Limits

Voltage drop is expressed as a percentage of the nominal system voltage:

```
Vd (%) = (Vd / V_line-to-line) × 100
```

Typical limits specified by clients or by electrical codes:

| Application | Maximum Voltage Drop |
|------------|---------------------|
| Transformer to main distribution board | 2–3% |
| Main distribution to sub-distribution | 2–3% |
| Final sub-circuit to load | 3–5% |
| Combined total (feeder + branch) | 5% maximum |

*These are typical values; always verify against project specifications or applicable national standards (NEC, BS 7671, etc.).*

### 4.4 Worked Voltage Drop Example

**Scenario:** 400A load at 400V three-phase, power factor 0.85, busbar run 50m, using aluminum flat busbar at 1,000A rating.

Manufacturer data for 1,000A aluminum flat busbar (4 × 80mm):
- `R = 0.034 mΩ/m` per phase
- `X = 0.016 mΩ/m` per phase (approximate, depends on spacing)

```
Vd = √3 × 400 × (0.034 × 0.85 + 0.016 × 0.527) × 50 / 1000
   = 1.732 × 400 × (0.0289 + 0.0084) × 50 / 1000
   = 692.8 × 0.0373 × 50 / 1000
   = 12.92 / 1000
   = 12.92V
   
Vd (%) = (12.92 / 400) × 100 = 3.23%
```

This is within a typical 5% limit. If it had exceeded 5%, options include:
- Selecting a larger busbar (reduces R and X)
- Improving power factor at the load
- Splitting the load across multiple shorter runs

---

## 5. Environmental Derating Factors

### 5.1 Temperature Derating

Busbar ampacity ratings are based on a reference ambient temperature. When the actual ambient temperature exceeds this reference, the busbar's heat dissipation capacity is reduced and the rated ampacity must be derated.

**For ambient temperatures above the reference (typically 30°C or 40°C):**

```
K_t = √((T_max - T_amb_actual) / (T_max - T_amb_reference))
```

Simplified typical values from IEEE C37.23 / NEMA BU1:

| Ambient Temperature (°C) | Temperature Derating Factor (K_t) |
|-------------------------|-----------------------------------|
| 30 | 1.00 |
| 35 | 0.97 |
| 40 | 0.94 |
| 45 | 0.91 |
| 50 | 0.88 |
| 55 | 0.84 |
| 60 | 0.80 |

*Values are typical for naturally cooled IPB/NSPB systems. Always consult the specific manufacturer's derating curves.*

**For ambient temperatures below reference:** Derating is generally not required for temperatures above 0°C, but note that condensation prevention measures become critical at low temperatures with high humidity.

### 5.2 Altitude Derating

At altitudes above 1,000m, air density decreases, reducing convective heat transfer from the busbar surface. The result is a higher operating temperature for a given load current.

**Typical altitude derating factor:**

| Altitude (m) | Altitude Derating Factor (K_a) |
|-------------|-------------------------------|
| ≤ 1,000 | 1.00 |
| 1,001–1,500 | 0.97 |
| 1,501–2,000 | 0.94 |
| 2,001–2,500 | 0.91 |
| 2,501–3,000 | 0.88 |
| > 3,000 | Consult manufacturer |

### 5.3 Combined Derating

When multiple derating factors apply simultaneously, the total derating factor is the **product of all individual factors**:

```
K_total = K_t × K_a × K_h × K_other
```

**Example:** A busbar installed at 45°C ambient and 1,800m altitude:

```
K_total = 0.91 × 0.94 = 0.855
```

The busbar's published ampacity rating must be multiplied by 0.855 to obtain the actual derated ampacity.

**Example — Applied Sizing:**

Design current: 8,000A

Manufacturer catalogue rating required:
```
I_rated_required = 8,000A / 0.855 = 9,357A
```

Select the next standard rating above 9,357A → typically 10,000A.

### 5.4 Harmonic Current Derating

Non-linear loads (variable frequency drives, UPS systems, servers, rectifiers) introduce harmonic currents into the busbar system. Harmonics increase heating in the neutral conductor and in the phase conductors due to skin effect and proximity effect, even when the fundamental-frequency current is within the busbar's rated ampacity.

**Harmonic current derating factors** (for busbar systems feeding significant non-linear loads):

| Total Harmonic Distortion (THD_i) | Derating Factor |
|----------------------------------|----------------|
| < 5% | 1.00 (no derating) |
| 5–15% | 0.90–0.95 |
| 15–25% | 0.85–0.90 |
| > 25% | Consult manufacturer / detailed analysis |

For data centers, server farms, or industrial facilities with large VFD populations, a harmonic analysis should be performed to determine appropriate derating or alternative busbar specifications.

---

## 6. Busbar Material and Profile Selection

### 6.1 Material Comparison

The two primary busbar materials are aluminum alloy and copper. The choice affects ampacity, mechanical properties, cost, weight, and installation practice.

| Property | Aluminum Alloy (6101-T61 / 6063-T42) | Copper (ETP / OFE) |
|---------|--------------------------------------|-------------------|
| Electrical conductivity | 61% IACS | 100% IACS |
| Density | 2.7 g/cm³ | 8.9 g/cm³ |
| Conductivity per unit weight | High | Moderate |
| Cost (material) | Lower | Higher (3–5× aluminum) |
| Thermal expansion | 23 × 10⁻⁶ /°C | 17 × 10⁻⁶ /°C |
| Typical use | Most IPB/NSPB applications | High-performance, space-constrained |
| Connections | Requires anti-oxidation compound | Easier silver-plating |

**For most power plant and industrial applications, aluminum alloy is the preferred busbar material** due to its favorable strength-to-weight ratio, adequate conductivity, corrosion resistance, and lower cost. Copper is reserved for specialized applications where superior conductivity is needed in a constrained space, or where connection practices favor copper.

### 6.2 Conductor Profile

**Tube (circular) conductors** are standard for IPB applications above approximately 3,000A. The annular cross-section provides:
- More uniform current distribution (reduces skin effect)
- Higher section modulus for equivalent cross-sectional area (better mechanical strength)
- Better heat dissipation per unit of conductive material

**Flat (rectangular) bus bars** are common in low-voltage switchgear, distribution panels, and NSPB systems at moderate current ratings. They are easier to branch-tap and more compact in low-voltage applications where the enclosure volume is not dominated by phase separation requirements.

### 6.3 Enclosure Design

For IPB and NSPB systems, the enclosure material and design affects:
- Electromagnetic shielding effectiveness
- Short-circuit fault current path capacity
- Corrosion resistance
- Weight

Aluminum enclosures are standard for most IPB applications due to their corrosion resistance, low weight, and excellent electromagnetic properties at power frequencies. Steel enclosures are used in specific applications where additional mechanical strength or magnetic shielding is required, though at the cost of higher weight.

---

## 7. Selection Checklist and Worked Example

### 7.1 Complete Sizing Checklist

Use this checklist to verify a complete and correct busbar specification:

**Electrical parameters:**
- [ ] Rated voltage (kV) — confirmed
- [ ] Maximum continuous load current (A) — established from load study
- [ ] Design current (A) — including growth margin and diversity
- [ ] Fault level at installation location (kA RMS) — from short-circuit study
- [ ] Fault clearing time (s) — coordinated with protective device settings
- [ ] Load power factor — for voltage drop calculation
- [ ] System frequency (Hz) — 50Hz or 60Hz

**Environmental conditions:**
- [ ] Minimum and maximum ambient temperature (°C)
- [ ] Altitude (m above sea level)
- [ ] Indoor or outdoor installation
- [ ] Corrosive atmosphere present? (salt spray, chemical, industrial)
- [ ] Solar radiation exposure (for outdoor or glasshouse installations)
- [ ] Harmonic load content (THD_i estimate)

**Installation parameters:**
- [ ] Busbar run length (m)
- [ ] Number and type of bends
- [ ] Minimum installation clearances
- [ ] Available space for busbar dimensions
- [ ] Structural support spacing

**Verification results:**
- [ ] Ampacity check: Busbar rating ≥ Design current / K_total ✓
- [ ] Short-circuit check: Icw ≥ I_available_RMS; Ipk ≥ 2.55 × I_available_RMS ✓
- [ ] Voltage drop check: Vd(%) ≤ applicable limit (typically 3–5%) ✓

### 7.2 Worked Sizing Example: 600MW Thermal Power Plant Unit Transformer Connection

**Given parameters:**
- System voltage: 24kV
- Generator full-load current: 14,437A (at 600MW, 24kV, 0.85pf)
- Maximum available short-circuit current: 100kA RMS
- Fault clearing time: 3s (generator breaker)
- Ambient temperature: 40°C
- Altitude: 50m (coastal, near sea level)
- Run length: 120m (generator to transformer)
- Power factor: 0.85
- Growth margin: 15%

**Step 1: Design current**
```
I_design = 14,437 × 1.15 × 0.95 = 15,772A
```
(0.95 diversity factor for well-loaded main bus; 15% growth margin)

**Step 2: Environmental derating**
```
K_total = 0.94 × 1.00 = 0.94
I_rated_required = 15,772 / 0.94 = 16,779A
```

**Step 3: Tentative selection — IPB, 24kV, 20,000A**
The next standard IPB rating above 16,779A is 20,000A. Verify short-circuit withstand.

**Step 4: Short-circuit verification**
```
Icw (rated) = 100kA / 3s ≥ I_available = 100kA RMS ✓
Ipk (rated) = 250kA ≥ 2.55 × 100 = 255kA — need 250kA or Ipk ≥ 255kA
```
*Check: Most 20,000A IPB systems have Ipk ratings of 250kA (which marginally equals or slightly exceeds 2.55 × 100kA = 255kA). For 100kA available fault, a 100kA/3s rated IPB with Ipk ≥ 250kA is adequate per IEEE C37.23.*

**Step 5: Voltage drop**
For a typical 20,000A IPB at 24kV, 120m run, at 14,437A load (0.85pf):
```
Approximate impedance: Z ≈ 0.015 mΩ/m per phase
Vd = √3 × 14,437 × 0.015 × 120 / 1000
   = 1.732 × 14,437 × 0.0018
   = 45.0V
Vd (%) = 45 / 24,000 × 100 = 0.19% ✓
```
(Well within the 3% limit for main feeder)

**Result:** Select 24kV, 20,000A IPB with 100kA/3s short-circuit rating.

> **Note:** This is a simplified example. Actual power plant IPB specification requires detailed coordination with the generator manufacturer, transformer manufacturer, switchgear vendor, and the EPC contractor's electrical design team. The short-circuit study must be project-specific, and all protective device coordination must be verified.

---

## 8. Frequently Asked Questions

### How do I calculate busbar size for a given current?

Calculate the design current (accounting for growth margin and diversity), then select a busbar with a continuous current rating at least 125% of this value after applying environmental derating factors. The three mandatory checks — ampacity, short-circuit withstand, and voltage drop — must all be satisfied. For a detailed step-by-step procedure, see Sections 2–4 of this handbook.

### What is the formula for busbar short-circuit withstand?

Short-circuit verification requires confirming two conditions: (1) `Icw_rated ≥ I_available_RMS` and (2) `Ipk_rated ≥ 2.55 × I_available_RMS` (for 50/60Hz systems with maximum DC offset). The busbar's rated Icw and Ipk values are published in manufacturer catalogues and must exceed the available fault current at the installation location, not merely the busbar's own rating.

### What is the derating factor for high altitude?

For altitudes above 1,000m, apply typical derating of approximately 0.4% per 100m above sea level (for natural convection cooled systems). At 1,800m, the derating factor is approximately 0.94. Combine this with temperature derating by multiplying the individual factors: `K_total = K_temperature × K_altitude`.

### How does power factor affect voltage drop in busbar?

Lower power factor increases the reactive component of voltage drop. The full voltage drop formula — `Vd = √3 × I × (R cos φ + X sin φ) × L` — accounts for both in-phase (resistive) and quadrature (reactive) components. At power factors below 0.8, using a simplified formula that neglects reactance can significantly underestimate voltage drop. Always use the full formula for low-power-factor loads.

### When do I need to derate for harmonic currents?

Derate for harmonic currents when the total harmonic distortion of current (THD_i) exceeds 5%. Non-linear loads (VFDs, UPS, servers, rectifiers) cause skin effect and proximity effect that increase heating above what the fundamental-frequency current alone would produce. For THD_i between 15% and 25%, typical derating factors of 0.85–0.90 apply. Above 25% THD_i, detailed harmonic analysis and manufacturer consultation are required.

### What is the difference between ampacity and current rating?

They refer to the same concept: the maximum continuous current a busbar can carry without exceeding its rated temperature limit under specified conditions. The term "ampacity" is common in North American practice (per NEC and IEEE); "current rating" is more commonly used in IEC standards and European practice. Both terms describe the same parameter.

### Can voltage drop limit alone determine busbar size?

No. Voltage drop is only one of three mandatory sizing checks. A busbar may pass the voltage drop check but fail ampacity or short-circuit checks. Conversely, a busbar with adequate ampacity and short-circuit rating may still produce excessive voltage drop in a long run, requiring a larger size. All three checks must always be performed.

---

## Conclusion

Rigorous busbar sizing requires three simultaneous checks — ampacity, short-circuit withstand, and voltage drop — applied in sequence and verified against the actual installation conditions. Environmental factors such as ambient temperature, altitude, and harmonic content routinely reduce the usable ampacity of catalogue-rated busbar systems, and failing to account for these reductions is the most common cause of busbar overheating in service.

For step-by-step selection guidance for IPB, NSPB, SPB, and cast resin busbar systems:
> [How to Choose the Right Busbar System for a Power Plant](./how-to-choose-the-right-busbar-system-for-a-power-plant.md)

For a comprehensive guide to each busbar type and their relative advantages:
> [Isolated Phase Busbar (IPB): Complete Technical Guide](./isolated-phase-busbar-ipb-guide.md) — The authoritative pillar page for all IPB-related technical content

For application-specific guidance by industry sector:
> [Where Are Busbar Systems Commonly Used?](./busbar-system-applications.md)

For a comprehensive reference to international standards (IEEE C37.23, IEC 61439-6, ATEX, NEC Article 368, and more):
> [Busbar Systems Standards and Compliance: Complete Engineering Guide](./busbar-systems-standards-compliance-guide.md)

For maintenance and troubleshooting guidance covering inspection schedules, thermal imaging, insulation testing, partial discharge monitoring, and fault diagnosis:
> [Busbar System Maintenance and Troubleshooting: Engineer's Complete Handbook](./busbar-maintenance-troubleshooting-engineers-handbook.md)

For a dedicated guide to LV busbar trunking for data centers — covering busway ampacity selection, short-circuit coordination, harmonic derating, and AI workload power distribution:
> [Data Center LV Busbar Trunking: Complete Selection and Design Guide](/blog/data-center-lv-busbar-trunking-selection-guide/)

---

*Last updated: April 11, 2026*
