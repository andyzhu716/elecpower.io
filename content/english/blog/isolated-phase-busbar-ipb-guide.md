---
title: "Isolated Phase Busbar (IPB): Complete Technical Guide"
description: "The definitive engineering guide to isolated phase busbar (IPB) systems. Covers technical principles, applications, selection criteria, and supplier evaluation for power plant and industrial projects."
date: 2026-04-09
lastmod: 2026-04-09
draft: false
tags:
  - isolated phase bus
  - IPB
  - busbar systems
  - power distribution
  - electrical engineering
  - technical guide
categories:
  - Technical Guide
  - Power Systems
featured_image: "images/blog/isolated-phase-busbar-ipb-guide.jpg"
og_image: ""
---

An **isolated phase busbar (IPB)** is a metal-enclosed electrical bus system in which each phase conductor occupies its own separate, grounded metallic housing. This design is the highest-reliability solution for high-current power transmission in critical infrastructure — particularly in power plants, large substations, and heavy industrial facilities where an unplanned outage carries severe financial or safety consequences.

This guide is the definitive technical reference for electrical engineers, EPC contractors, and procurement specialists evaluating or specifying IPB systems. It covers the engineering principles behind IPB, how it compares to alternative busbar technologies, where it is applied, and how to select and specify the right IPB system for your project.

**Key Takeaways:**
- IPB provides complete phase-to-phase fault elimination through physically isolated enclosures for each phase
- IPB is the standard choice for generator connections in power plants above 100MW
- Short-circuit withstand ratings up to 300kA (3s) and peak ratings up to 750kA are achievable
- IPB service life exceeds 40 years with minimal maintenance under normal operating conditions
- Specifying the correct IPB requires matching electrical ratings, environmental conditions, and applicable standards

---

## Table of Contents

1. [What Is Isolated Phase Busbar?](#1-what-is-isolated-phase-busbar)
2. [Technical Principles](#2-ipb-technical-principles)
3. [IPB vs Other Busbar Types](#3-ipb-vs-other-busbar-types)
4. [Applications and Industries](#4-applications-and-industries)
5. [Selection and Sizing Guide](#5-selection-and-sizing-guide)
6. [Wetown IPB Solutions](#6-wetown-ipb-solutions)
7. [Related Resources](#7-related-resources)
8. [Frequently Asked Questions](#8-frequently-asked-questions)

---

## 1. What Is Isolated Phase Busbar?

### 1.1 Definition and Core Concept

An isolated phase busbar (IPB) is a type of high-current electrical bus system in which each of the three phase conductors (A, B, and C) is enclosed in its own separate, continuously grounded metallic housing. The enclosures are typically aluminum alloy, though steel enclosures are used in specific applications. Each phase housing is electrically isolated from the others, hence the name "isolated phase."

The fundamental purpose of IPB is to **eliminate the possibility of phase-to-phase faults** within the bus system itself. Because each phase lives in its own grounded enclosure, a fault on one phase cannot propagate to another. This single design characteristic is the reason IPB is mandated or strongly preferred in the most critical power delivery applications worldwide.

### 1.2 Historical Background

Isolated phase bus technology emerged in the mid-20th century as power plant generating capacities grew beyond what conventional busbar systems could reliably handle. As generator ratings increased from tens of megawatts to hundreds and eventually over 1,000 megawatts, the fault currents involved became large enough to cause catastrophic damage in conventional bus systems.

The first IPB installations appeared in large thermal and nuclear power plants in North America and Europe during the 1950s and 1960s. Early designs used steel enclosures; aluminum became the dominant material by the 1970s due to its superior corrosion resistance, lighter weight, and better electromagnetic properties at power frequencies. Today, IPB is a mature, standardized technology used globally.

### 1.3 Why IPB Is Essential for Large Power Plants

Modern large-scale power generation depends on IPB for several irreplaceable reasons:

**High fault currents.** A 1,000MW generator operating at 24kV produces a full-load current of approximately 24,000A. A three-phase fault at the generator terminals could produce symmetrical short-circuit currents of 150kA to 300kA or more. No other busbar technology can safely carry and distribute such currents over the distances involved in a typical power plant layout.

**Operational reliability.** Power plants are expected to operate for 40 to 60 years. An IPB system, properly specified and installed, will outlast virtually every other component in the plant with minimal maintenance. The cost of an unplanned outage — in lost generation revenue, replacement power purchases, and potential contractual penalties — vastly exceeds the incremental cost of specifying IPB.

**Electromagnetic compatibility.** The grounded metal enclosures of IPB provide excellent electromagnetic shielding. This prevents induced currents in nearby steel structures (which would cause heating and energy losses) and reduces electromagnetic interference with nearby instrumentation and communication systems.

**Generator protection.** The generator is among the most expensive and most critical assets in a power plant. IPB provides a controlled, predictable electrical environment for the generator-circuit breaker-transformer interface, minimizing stress on the generator and its associated protection systems.

### 1.4 Key Standards Governing IPB

IPB systems are designed and tested to internationally recognized standards that define the requirements for construction, performance, and quality assurance:

| Standard | Title | Region |
|----------|-------|--------|
| **IEEE C37.23** | IEEE Standard for Metal-Enclosed Bus | International |
| **IEC 62271-212** | High-voltage switchgear and controlgear — Metal-enclosed bus | International |
| **UL 857** | Standard for Busways | United States |
| **NEMA BU1** | Metal-Enclosed Bus | United States |
| **GB/T 8349** | Metal-enclosed bus | China |
| **IEEE 693** | Seismic Design of Substations | International (seismic applications) |

For nuclear power plants, additional standards such as **IEEE 344** (seismic qualification for Class 1E equipment) apply. For petrochemical and hazardous area installations, **IEEE 841** and applicable area classification standards may be required.

> **Learn more:** [Busbar Systems Standards and Compliance: Complete Engineering Guide](./busbar-systems-standards-compliance-guide.md)

---

## 2. IPB Technical Principles

### 2.1 Construction and Design

A complete IPB system consists of multiple functional components, each designed to work together to deliver reliable high-current power transmission.

#### Phase Conductors

The phase conductor is the current-carrying element at the core of each IPB phase enclosure. Conductor design has evolved significantly since the first IPB installations:

**Material.** Aluminum alloy (typically 6101-T61 or 6063-T42) is the predominant conductor material in modern IPB systems. Aluminum offers an excellent balance of electrical conductivity (approximately 61% of copper), mechanical strength, corrosion resistance, and cost. Copper conductors are used in specialized applications where superior conductivity is required, but copper's higher cost and weight typically make aluminum the preferred choice for most installations.

**Profile.** Conductor cross-sections vary by manufacturer and application. Common profiles include:
- **Circular (tube) conductors** — The most common profile, offering uniform current distribution, good mechanical strength, and ease of fitting tap points and branch connections
- **Rectangular (flat) bus bars** — Used in lower-current sections or where space constraints favor a flat profile
- **Hollow conductors** — Used in very high current applications (typically above 15,000A) where skin effect considerations favor an annular cross-section

**Sizing.** Conductor cross-section is determined by the required continuous current rating, accounting for the conductor material's resistivity, the permissible temperature rise, and heat dissipation conditions. Conductor size is typically expressed in terms of current density (A/mm²) at the design operating conditions. Modern IPB conductors operate at current densities of 1.5 to 3.0 A/mm² depending on cooling method and enclosure design.

#### Phase Enclosures

Each phase conductor is housed within a continuous, grounded metallic enclosure. The enclosure serves multiple functions:

**Electromagnetic shielding.** The grounded enclosure acts as a conductive shield that contains the electromagnetic field generated by the phase current within the enclosure. This prevents the external magnetic fields that would otherwise induce heating in nearby steel structures (reactor hold-down beams, building steel, pipe supports) and reduces electromagnetic interference with nearby instrumentation cables.

**Mechanical protection.** The enclosure provides physical protection for the conductor and insulation system from impact, contamination, and environmental exposure.

**Grounding and fault current path.** The enclosure is solidly bonded to ground at multiple points along the run and at all termination points. Under fault conditions, the enclosure carries significant induced currents that are safely returned to ground. The enclosure must have sufficient cross-section to serve as an adequate fault current path without suffering thermal or mechanical damage.

Enclosure dimensions are determined by the required phase-to-phase and phase-to-ground clearances, which in turn are governed by the system voltage and the required dielectric withstand capability.

#### Insulators and Supports

The phase conductor is supported within its enclosure by insulating spacers and support insulators. These components must:

- Provide adequate electrical insulation between the live conductor and the grounded enclosure
- Mechanically support the conductor against its own weight plus electromagnetic forces during fault conditions
- Accommodate thermal expansion and contraction of the conductor without transferring excessive loads to the enclosure
- Maintain their electrical and mechanical properties over the full design life of the installation

Insulator materials include ceramic, fiberglass-reinforced epoxy (FRE), and cycloaliphatic epoxy. The choice depends on the electrical stress, mechanical loading, environmental conditions, and manufacturer preferences.

#### Expansion Joints

IPB systems include bellows-type expansion joints at regular intervals along straight runs and at all termination points. Expansion joints serve two critical functions:

1. **Thermal expansion accommodation.** As the conductor heats from I²R losses and from solar gain (for outdoor installations), it expands. Expansion joints prevent the development of large compressive or tensile stresses in the conductor system that could cause buckling, joint separation, or insulator damage.

2. **Seismic and dynamic movement accommodation.** In seismically active regions, expansion joints allow the enclosure and conductor to move independently during an earthquake event, reducing mechanical stress on insulators and terminations.

Expansion joints are typically specified every 10 to 20 meters on straight runs, with additional joints at generator and transformer terminations.

#### Connection Points and Terminations

IPB systems require specialized termination structures at each interface with other equipment:

- **Generator connection housing** — A flexible or semi-flexible connection assembly that accommodates generator terminal movement during startup, shutdown, and load changes while maintaining electrical continuity
- **Transformer bushings** — Sealed entries through the transformer tank wall, incorporating a transition from the IPB conductor to the transformer's internal leads
- **Switchgear connections** — Hard-drawn connections to the generator circuit breaker's isolated phase bus or to the unit transformer
- **Branch circuit connections** — Taps for auxiliary circuits such as excitation transformers, potential transformers, and unit auxiliary transformers

### 2.2 Electrical Characteristics

#### Current Ratings

IPB systems are manufactured in a wide range of continuous current ratings to match specific project requirements:

| Rating Range | Typical Application |
|--------------|---------------------|
| 1,200A – 3,000A | Small generators, auxiliary connections |
| 3,000A – 10,000A | Medium-sized generators (100–400MW) |
| 10,000A – 20,000A | Large generators (400–800MW) |
| 20,000A – 30,000A+ | Ultra-large generators (800–1,000MW+) |
| Up to 50,000A | Custom super-high-current applications |

The continuous current rating is determined under defined test conditions (typically 40°C ambient temperature, sea level, natural convection cooling). The rating must be adjusted downward (derated) for conditions that reduce heat dissipation:

- Ambient temperatures above 40°C: typically derate by 0.5% per °C above 40°C
- Altitudes above 1,000m: typically derate by approximately 0.4% per 100m above 1,000m
- Enclosure heating from external sources (adjacent equipment, solar radiation)

#### Short-Circuit Withstand Ratings

Short-circuit withstand is among the most critical IPB specifications. Under fault conditions, the electromagnetic forces on the conductors and enclosures can be enormous — proportional to the square of the instantaneous fault current. A 200kA RMS fault current produces peak electromagnetic forces exceeding several thousand newtons per meter on the conductor assembly.

IPB short-circuit ratings are specified as:

- **Short-time withstand current (Icw)** — The RMS value of current the bus can carry for a specified duration (typically 1s or 3s) without suffering electrical or mechanical damage. Expressed in kA RMS.
- **Peak withstand current (Ipk)** — The maximum instantaneous peak current the bus can withstand without mechanical failure. Expressed in kA peak. Typically 2.5 to 2.7 times the RMS short-circuit current for 50/60Hz systems.

Common short-circuit withstand ratings include:

| Rating | Typical Use |
|--------|-------------|
| 40kA / 3s | Auxiliary and distribution applications |
| 63kA / 3s | Medium-sized plant unit connections |
| 100kA / 3s | Large generator connections |
| 200kA / 3s | Ultra-large generator connections |
| Up to 300kA / 3s | Custom super-large units |

#### Voltage Ratings

IPB systems are designed for specific voltage classes, with insulation coordination to match:

| Voltage Class | Typical Use | BIL (Basic Impulse Level) |
|--------------|-------------|--------------------------|
| 6.6kV / 7.2kV | Small generators, motors | 60–75kV |
| 10kV / 12kV | Medium generators | 75–95kV |
| 13.8kV / 15kV | Standard large generators (US) | 95–110kV |
| 24kV | High-voltage generators, large units | 125–150kV |
| 35kV | Limited applications | 150–185kV |

The insulation system must be coordinated with system overvoltage protection (surge arresters) and must account for switching transients as well as lightning impulse stress.

### 2.3 IPB vs Other Busbar Types

Choosing between IP and other busbar technologies is one of the most important decisions in power distribution system design. The choice affects capital cost, reliability, maintenance requirements, and operational risk over the entire life of the installation.

> **Detailed comparison:** [IPB vs Enclosed Busbar: What's the Difference?](./ipb-vs-enclosed-busbar.md)
> 
> **Learn about alternatives:** [What Is Isolated Phase Bus and How Does It Work?](./what-is-isolated-phase-bus.md)

**Decision framework at a glance:**

| Application Requirement | Recommended Technology |
|------------------------|----------------------|
| Generator connection, >300MW unit | IPB |
| Generator connection, 100–300MW unit | IPB or SPB |
| Medium-voltage distribution, 1,000–6,000A | NSPB or SPB |
| Low-voltage distribution, <1,000A | Enclosed busbar or cable |
| Complex routing, retrofit, tight spaces | Cable bus |
| Harsh environment (corrosive, wet) | CRB (cast resin busway) |

**For a comprehensive guide to selecting the right busbar system for your project:**
> [How to Choose the Right Busbar System for a Power Plant](./how-to-choose-the-right-busbar-system-for-a-power-plant.md)

---

## 3. IPB vs Other Busbar Types

This section provides a detailed comparative analysis of IPB against the other principal busbar technologies: non-segregated phase bus (NSPB), segregated phase bus (SPB), cast resin busway (CRB), and cable bus.

### 3.1 IPB vs Non-Segregated Phase Bus (NSPB)

**Non-segregated phase bus (NSPB)** houses all three phase conductors within a common, single enclosure without physical barriers between phases. All three phases share the same grounded housing.

| Feature | IPB | NSPB |
|---------|-----|------|
| Phase separation | Each phase in its own enclosure | All phases in common enclosure |
| Phase-to-phase fault risk | Virtually eliminated | Possible (low probability but non-zero) |
| Maximum current rating | 50,000A+ | 6,300A |
| Maximum voltage | 35kV+ | 40.5kV |
| Short-circuit withstand | Up to 300kA | Up to 100kA |
| Enclosure shielding | Individual, optimized per phase | Shared, less effective |
| Space requirement | Greater (3× single-phase runs) | Compact (single three-phase run) |
| Capital cost | Higher | Lower |
| Weight | Higher | Lower |
| Installation complexity | Higher | Lower |
| Maintenance | Minimal | Moderate |

**When to choose NSPB over IPB:** NSPB is appropriate for medium-voltage distribution applications where the current and fault levels are moderate (typically below 6,300A and 100kA), space is at a premium, and the cost sensitivity is high. NSPB is commonly used in auxiliary power systems in power plants, medium-voltage switchgear bus connections, and industrial plant substation buswork.

### 3.2 IPB vs Segregated Phase Bus (SPB)

**Segregated phase bus (SPB)** uses metal barriers to divide a common enclosure into three separate phase compartments. Each phase is isolated from its neighbors by a solid metal partition, but all three share the overall housing.

| Feature | IPB | SPB |
|---------|-----|-----|
| Phase separation | Separate enclosures (fully isolated) | Common enclosure with phase barriers |
| Phase-to-phase fault risk | Virtually eliminated | Very low (barriers prevent most faults) |
| Maximum current rating | 50,000A+ | 15,000A |
| Space requirement | Greatest (3× independent runs) | Moderate |
| Cost | Highest | Moderate |
| Maximum fault withstand | Up to 300kA | Up to 100–130kA |

**When to choose SPB over IPB:** SPB fills the gap between IPB and NSPB, offering better phase isolation than NSPB while being more compact and economical than IPB. SPB is well-suited for medium-power applications in the 4,000A to 10,000A range, auxiliary transformer connections, and industrial plant medium-voltage buswork where IPB's cost is not justified but NSPB's fault performance is inadequate.

### 3.3 IPB vs Cast Resin Busway (CRB)

**Cast resin busway (CRB)** uses fully cast epoxy resin as the insulation and outer housing for the phase conductors. There is no air gap; the conductor is fully encapsulated.

| Feature | IPB | CRB |
|---------|-----|-----|
| Insulation type | Air with spacer insulators | Fully cast epoxy resin |
| Maximum voltage | 35kV+ | 35kV |
| Maximum current | 50,000A+ | 6,300A |
| IP rating | IP54–IP65 | IP68 (submersible) |
| Fire resistance | Metal housing, depends on coating | F120 (120-minute fire rating) |
| Maintenance | Low (accessible internals) | Near-zero (solid cast construction) |
| Corrosion resistance | Moderate (depends on enclosure) | Excellent (epoxy encapsulation) |
| Installation flexibility | Rigid, straight runs | Good flexibility in routing |
| Cost | Higher at high currents | Competitive at medium currents |

**When to choose CRB over IPB:** CRB excels in environments where the IPB enclosure would be at risk — corrosive atmospheres (coastal, chemical plants), outdoor installations with potential flooding, and areas requiring explosion-proof equipment. CRB's maintenance-free, solid-insulation construction is particularly valued in harsh industrial environments and in applications where periodic inspection of current-carrying parts is impractical.

### 3.4 IPB vs Cable Bus

**Cable bus** uses multiple parallel insulated cables per phase instead of rigid bus bars. Cables are installed in a tray, conduit, or mesh support system.

| Feature | IPB | Cable Bus |
|---------|-----|-----------|
| Conductor type | Rigid aluminum/copper bars | Multiple insulated cables per phase |
| Flexibility | Rigid, fixed routing | Highly flexible routing |
| Complex routing suitability | Poor (bends have large minimum radii) | Excellent |
| Current rating | Up to 50,000A+ | Typically up to 5,000–6,000A |
| Voltage drop | Lower (larger cross-section) | Higher (cable reactance) |
| Fault current capability | Excellent | Limited by cable thermal withstand |
| Maintenance | Low | Moderate (multiple cable terminations) |
| Installation time | Longer for complex layouts | Shorter for complex routing |

**When to choose cable bus over IPB:** Cable bus is the preferred choice for applications with complex routing — multiple direction changes, existing structural obstacles, retrofit installations, or connections across equipment that cannot be moved. Cable bus is also typically more economical for moderate current levels (below approximately 4,000A) where the full capabilities of IPB are not required.

---

## 4. Applications and Industries

### 4.1 Power Generation

Power plants are the primary market for IPB systems. The high generating capacities and associated fault currents in modern power plants make IPB the only technically appropriate solution for the generator circuit.

#### Thermal Power Plants (Coal, Oil, Gas)

In thermal power plants, IPB connects the generator output to the unit transformer and auxiliary systems. A typical 1,000MW ultra-supercritical coal-fired unit generates at 27kV with full-load current of approximately 21,400A and potential fault currents of 150–250kA. No alternative busbar technology can safely handle these conditions at reasonable cost and reliability.

The IPB run in a large thermal plant typically includes:
- Generator lead section (generator terminal box to generator circuit breaker)
- Main bus section (breaker to unit transformer)
- Branch connections to excitation transformer, neutral grounding equipment, and unit auxiliary transformer

#### Nuclear Power Plants

Nuclear plants impose the most demanding requirements on IPB systems due to their extremely high reliability requirements and the unique environmental conditions in nuclear containments. IPB in nuclear plants is typically specified to:

- IEEE 693 seismic design requirements (Required Performance Level for seismic Category 1 equipment)
- IEEE 344 seismic qualification testing
- Enhanced quality assurance programs per 10 CFR 50 Appendix B or equivalent
- Stringent material traceability requirements for pressure-retaining components

The IPB routing in a nuclear plant often passes through containment penetrations, which require special sealed penetration designs rated for the containment pressure boundary.

#### Hydroelectric Power Plants

Hydroelectric generators are often located in caverns or outdoor environments with high humidity and potentially corrosive water spray. IPB for hydro applications must account for:

- High humidity and condensation risk (requiring ACDU or equivalent anti-condensation systems)
- Potentially seismically active locations (many large hydro projects are in mountainous regions)
- Long horizontal runs from outdoor generators to indoor switchyards

#### Pumped Storage

Pumped storage hydro plants have unique operational requirements: the generator-motors start and stop frequently (sometimes multiple times per day) and operate in both generation and pumping modes. This cyclic loading places additional thermal and mechanical stress on IPB systems compared to conventional thermal plants, which typically run at near-constant output for extended periods.

> **Learn more:** [Where Are Busbar Systems Commonly Used?](./busbar-system-applications.md)

### 4.2 Large Industrial Facilities

Beyond power generation, IPB serves critical power distribution functions in heavy industry:

#### Steel and Metal Smelting

Aluminum smelters, copper refineries, and steel mills operate electrolytic processes requiring DC power at extremely high currents — commonly 50,000A to 300,000A+ per potline. While these are DC systems using rectifier-transformer-bus assemblies, AC IPB is used in the upstream AC distribution network feeding the rectifier transformers.

#### Petrochemical and Chemical Plants

Large refineries and chemical complexes operate continuous processes where an unplanned outage can cause extensive economic damage through lost production, restart costs, and potential safety incidents. IPB is specified for:

- Main substation to process area power distribution
- Large motor feeder connections (drives for compressors, pumps, fans)
- Cogeneration plant connections in combined heat and power (CHP) installations

#### Data Centers

While most data center power distribution operates at voltages and currents where enclosed busbar suffices, hyper-scale facilities operated by major cloud providers (Google, Microsoft Azure, Amazon AWS) can have power demands exceeding 100MW at a single campus. At these scales, IPB may be used for:

- Utility substation to main switchgear connections
- Generator backup system connections in mission-critical facilities
- Inter-building distribution at multi-building campuses

### 4.3 Grid Infrastructure

IPB is used in transmission and distribution substations at voltage levels from 115kV to 500kV for high-current bus connections, particularly where generator-level fault currents must be accommodated.

### 4.4 Marine and Offshore

Large vessels, offshore oil and gas platforms, and offshore wind substations operate in corrosive salt spray environments with high vibration and seismic or motion loading. Marine IPB is specified to additional standards including IEC 60092 and classification society rules (DNV, ABS, Lloyd's Register).

> [How to Prevent Condensation in Enclosed Busbar Systems](./how-to-prevent-condensation-in-enclosed-busbar-systems.md) — Essential reading for humid and marine environments.

---

## 5. Selection and Sizing Guide

### 5.1 Key Selection Parameters

Selecting the correct IPB system requires gathering the following information:

**Electrical parameters:**
- Rated voltage (kV)
- Maximum continuous load current (A)
- Future load growth allowance (%)
- System frequency (Hz)
- Maximum available short-circuit current at the installation location (kA RMS)
- Duration of the short-circuit current for thermal withstand (typically 1s or 3s)
- Peak short-circuit current (kA peak)

**Environmental conditions:**
- Minimum and maximum ambient temperature (°C)
- Altitude (m above sea level)
- Indoor or outdoor installation
- Presence of corrosive substances (salt spray, chemical fumes)
- Seismic design requirements (yes/no; if yes, required seismic level)
- Explosion-proof or hazardous area requirements

**Installation information:**
- Single-line diagram showing IPB routing
- Required bus run length (m)
- Number and type of bends (horizontal and vertical)
- Termination details for connected equipment
- Available space for IPB routing
- Special routing requirements (wall penetrations, cable trays in same area)

### 5.2 Sizing Procedure

**Step 1: Determine required continuous current rating**

Calculate the design current:

```
I_design = I_max × (1 + growth_factor) × derating_factor
```

Where:
- `I_max` = maximum expected continuous load current (A)
- `growth_factor` = allowance for future load growth (typically 10–25%)
- `derating_factor` = factor to account for ambient temperature and altitude

Standard practice is to specify a bus rated for at least 125% of the calculated design current, providing a margin for measurement uncertainty and temporary overloads.

**Step 2: Verify short-circuit withstand**

The IPB short-circuit rating must exceed the maximum available fault current at the installation point:

```
Icw_required ≥ I_available_fault_RMS
Ipk_required ≥ 2.5 × I_available_fault_RMS
```

If the available fault current exceeds the standard IPB short-circuit ratings available from manufacturers, consider:
- Adding series reactance to limit fault current (at the cost of increased voltage drop)
- Selecting a higher-rated IPB system
- Upstream system modifications to reduce fault levels

**Step 3: Verify insulation coordination**

The IPB insulation level (BIL, power frequency withstand) must be coordinated with:
- System nominal voltage
- Surge arrester protective level at the installation location
- Expected switching and lightning impulse overvoltages

**Step 4: Check environmental derating**

If the installation conditions differ from the IPB standard rating conditions, apply appropriate derating factors. Common derating scenarios include:

| Condition | Typical Derating |
|-----------|-----------------|
| Ambient temperature 40–50°C | -0.5% per °C above 40°C |
| Altitude 1,000–3,000m | -0.4% per 100m above 1,000m |
| Altitude above 3,000m | Consult manufacturer |
| Solar heating (outdoor) | -5% to -15% depending on installation |

### 5.3 Specification Checklist

Before issuing a specification or request for quotation, verify that the following information is included:

- [ ] Rated voltage and frequency
- [ ] Continuous current rating (with derating assumptions stated)
- [ ] Short-circuit withstand rating (Icw and Ipk) with duration
- [ ] Required insulation level (BIL)
- [ ] Ambient temperature range
- [ ] Altitude
- [ ] Indoor/outdoor installation
- [ ] Seismic requirements
- [ ] Corrosion/international environment requirements
- [ ] Applicable standards (IEEE, IEC, GB/T, etc.)
- [ ] Required factory tests
- [ ] Documentation requirements (drawings, calculations, test reports)
- [ ] Delivery and installation schedule

---

## 6. Wetown IPB Solutions

Wetown Electric Group (Stock Code: 688226) is a leading global manufacturer of isolated phase busbar systems with decades of engineering and manufacturing experience serving power plants and heavy industrial facilities worldwide.

### 6.1 Product Range

Wetown's IPB product line covers the full range of power plant and industrial applications:

| Product | Voltage | Current Rating | Key Applications |
|---------|---------|---------------|------------------|
| **Standard IPB** | 10–24kV | 3,000–30,000A+ | Thermal, nuclear, hydro plants |
| **High-Current IPB** | 10–35kV | 30,000–50,000A+ | Ultra-large generators, smelters |
| **Seismic Qualified IPB** | 10–24kV | 3,000–25,000A | Nuclear, seismically active regions |
| **Outdoor IPB** | 10–35kV | 3,000–30,000A+ | Outdoor switchyards,沿海/户外 |
| **Harsh Environment IPB** | 10–24kV | 3,000–20,000A | Coastal, chemical, offshore |

### 6.2 Auxiliary Equipment

Complete IPB systems require supporting equipment that ensures stable, safe, long-term operation:

- **PT & LA Cubicle** — Potential transformer and lightning arrester cabinet providing voltage monitoring, overvoltage protection, and metering functions for the generator bus circuit
- **Neutral Grounding Cabinet (NGC)** — High-resistance grounding system that limits fault currents and provides ground fault detection and indication
- **Air Circulation Drying Unit (ACDU)** — Micro-positive pressure system that maintains dry air inside IPB enclosures, preventing condensation in humid environments

### 6.3 Quality and Certification

Wetown's IPB manufacturing is conducted under a comprehensive quality management system certified to ISO 9001, with products tested to IEEE C37.23, IEC 62271-212, and applicable regional standards. Factory testing includes:

- Dielectric withstand testing (power frequency and impulse)
- Resistance and continuity verification
- Dimensional verification
- Visual and mechanical inspection

### 6.4 Global Project Experience

Wetown has supplied IPB systems to power projects across Asia, the Middle East, Africa, and South America, with reference projects ranging from 100MW to 1,000MW+ generating units. Contact the Wetown technical team to discuss your project requirements.

---

## 7. Related Resources

### Technical Guides

- [What Is Isolated Phase Bus and How Does It Work?](./what-is-isolated-phase-bus.md) — Foundational introduction to IPB technology
- [IPB vs Enclosed Busbar: What's the Difference?](./ipb-vs-enclosed-busbar.md) — Detailed technical comparison with alternative busbar technologies
- [IPB vs NSPB: What's the Difference?](./ipb-vs-nspb.md) — Detailed comparison of isolated phase vs non-segregated phase bus
- [Busbar Sizing and Selection: Engineer's Handbook](./busbar-sizing-selection-engineers-handbook.md) — **NEW** — Step-by-step ampacity calculation, short-circuit verification, and voltage drop analysis for all busbar types

### Application Guides

- [Where Are Busbar Systems Commonly Used?](./busbar-system-applications.md) — Industry-specific applications across power generation, industrial, and infrastructure sectors
- [How to Choose the Right Busbar System for a Power Plant](./how-to-choose-the-right-busbar-system-for-a-power-plant.md) — Decision framework for selecting the appropriate busbar technology for your project
- [How to Prevent Condensation in Enclosed Busbar Systems](./how-to-prevent-condensation-in-enclosed-busbar-systems.md) — Anti-condensation solutions for IPB and NSPB systems

### Standards Reference

- [Busbar Systems Standards and Compliance: Complete Engineering Guide](./busbar-systems-standards-compliance-guide.md) — Comprehensive guide to IEEE C37.23, IEC 61439-6, ATEX/IECEx, UL 857, NEC Article 368, GB/T 8349, and other applicable standards for engineers and specifiers

---

## 8. Frequently Asked Questions

### What is the difference between IPB and NSPB?

The key difference is the degree of phase isolation. In IPB, each phase conductor is housed in its own separate, grounded metallic enclosure. In NSPB (non-segregated phase bus), all three phase conductors share a common three-phase enclosure without physical barriers between phases. IPB provides superior fault protection and higher current and fault ratings; NSPB is more compact and economical but cannot eliminate phase-to-phase faults within the bus itself. [Learn more about the differences](./ipb-vs-nspb.md).

### What current ratings are available for IPB?

IPB systems are manufactured in continuous current ratings ranging from approximately 1,200A to over 50,000A. Standard product lines from major manufacturers typically cover 3,000A to 30,000A, with custom designs available above this range for super-high-current applications such as aluminum smelters.

### How do you size an IPB system?

IPB sizing involves three key checks: (1) continuous current rating must be at least 125% of the maximum expected load current, with derating for ambient temperature and altitude; (2) short-circuit withstand rating must exceed the maximum available fault current at the installation location; (3) insulation level must be coordinated with system voltage and surge protection. Download our [selection checklist](#) for a complete step-by-step sizing procedure.

### What standards govern IPB design and testing?

The primary international standards are IEEE C37.23 (IEEE Standard for Metal-Enclosed Bus) and IEC 62271-212 (High-voltage switchgear and controlgear — Metal-enclosed bus). Additional standards may apply depending on application, region, and customer requirements. [See our full standards guide](./busbar-systems-standards-compliance-guide.md).

### Can IPB be installed outdoors?

Yes. Outdoor IPB systems are designed with weatherproof enclosures featuring enhanced sealing, sun shields to reduce solar heating, and provisions for condensation management. Outdoor installations typically cost 10–20% more than equivalent indoor systems due to the additional environmental protection required.

### What maintenance does IPB require?

IPB requires minimal maintenance compared to other electrical equipment. Recommended maintenance activities include: annual visual inspection for signs of overheating, corrosion, or damage; periodic infrared thermographic surveys to identify abnormal hot spots; torque verification of bolted connections every 3–5 years; and insulation resistance testing as part of periodic electrical maintenance programs. With proper installation, IPB systems routinely operate for 40+ years with minimal maintenance.

### What is the typical delivery time for an IPB system?

Delivery times vary by order complexity and manufacturer workload. Typical delivery times for standard IPB systems range from 8 to 16 weeks from order confirmation to shipment. Complex systems with custom ratings, extensive non-standard routing, or requiring seismic qualification may require 20 to 30 weeks. Early engagement with the manufacturer during the engineering design phase is recommended to ensure timely delivery aligned with project construction schedules.

### How does IPB perform in seismic environments?

IPB systems can be designed and qualified to withstand seismic events. Seismic qualification is performed per IEEE 693 (IEEE Standard for Seismic Design of Substations) or equivalent regional seismic standards. Qualification methods include analytical analysis, shake table testing, or a combination of both. For nuclear power plants and other critical facilities in seismically active regions, seismic qualification is a standard requirement.

---

## Conclusion

Isolated phase busbar systems are the definitive solution for high-current power distribution in critical applications. The complete phase isolation they provide — eliminating the possibility of phase-to-phase faults within the bus system itself — makes IPB the only technically appropriate choice for generator connections in power plants above 100MW and for the most demanding industrial applications.

Successful IPB implementation requires careful attention to specification, design coordination, installation quality, and compliance with applicable standards. The investment in proper IPB specification and quality assurance is returned many times over in the form of decades of reliable, maintenance-light service.

For project-specific technical consultation, IPB pricing, or to discuss your power distribution requirements, contact the Wetown Electric technical team.

For a comprehensive reference to all international standards applicable to busbar systems:
> [Busbar Systems Standards and Compliance: Complete Engineering Guide](./busbar-systems-standards-compliance-guide.md)

For maintenance and troubleshooting guidance covering inspection schedules, thermal imaging, partial discharge monitoring, and fault diagnosis:
> [Busbar System Maintenance and Troubleshooting: Engineer's Complete Handbook](./busbar-maintenance-troubleshooting-engineers-handbook.md)

For a dedicated guide to LV busbar trunking used in data centers and commercial facilities — covering open channel vs enclosed busway, tap-off unit design, N+1/2N redundancy, and AI workload power distribution:
> [Data Center LV Busbar Trunking: Complete Selection and Design Guide](/blog/data-center-lv-busbar-trunking-selection-guide/)

---

*Last updated: April 11, 2026*
