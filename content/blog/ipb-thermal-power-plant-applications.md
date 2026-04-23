---
title: "Isolated Phase Bus (IPB) in Thermal Power Plants: Engineering Applications Guide"
description: "A comprehensive engineering guide to IPB (isolated phase bus) applications in thermal power plants. Covers generator connections, auxiliary systems, switchgear interfaces, and key design considerations for 300MW–1000MW class units."
meta_title: "IPB Applications in Thermal Power Plants | Wetown"
date: 2026-04-23
draft: false
categories: ["IPB Applications", "Power Plant"]
tags: ["IPB", "thermal power plant", "火电厂", "generator connection", "busbar application"]
keywords: ["IPB thermal power plant", "火电厂离相母线", "generator isolated phase bus", "power plant busbar connection", "IPB 300MW 600MW 1000MW"]
---



# Isolated Phase Bus (IPB) in Thermal Power Plants: Engineering Applications Guide

Isolated Phase Bus (IPB) is the dominant busbar technology for high-current electrical connections in thermal power plants. In units ranging from 300 MW to 1,000 MW and beyond, IPB serves as the critical link between the generator and the main transformer — a connection that must carry tens of thousands of amps fault-free for decades.

This article provides an engineering-focused guide to IPB applications in thermal power plants. It covers the primary connection scheme, auxiliary system interfaces, civil structure coordination, environmental design considerations, and key factors that plant designers and EPC contractors need to verify with IPB suppliers.

---

## 1. Why Thermal Power Plants Require IPB

### 1.1 Scale of Fault Currents

A 600 MW generator operating at 20 kV generates a full-load current of approximately 17,320 A. During a three-phase bolted fault at the generator terminals, the initial symmetrical short-circuit current can reach 150 kA to 250 kA, with peak electromagnetic forces exceeding several tonnes per metre between phase conductors.

No other busbar technology can safely contain and transmit these fault levels within the physical layout of a power plant while maintaining the phase isolation that prevents fault propagation.

### 1.2 Operational Life Matching Plant Design Life

A modern thermal power plant is designed for an operational life of 30 to 50 years. IPB, when properly specified and installed, will typically outlast the plant with minimal intervention. This makes IPB a lifecycle cost winner despite its higher initial capital cost.

### 1.3 Grid Code Compliance

In most jurisdictions, power plants must meet grid connection codes that mandate specific fault ride-through capabilities and stability performance. The generator-circuit breaker-transformer interface — bridged by IPB — must maintain electrical integrity throughout these transient events.

---

## 2. Primary IPB Connection Scheme in Thermal Power Plants

### 2.1 Generator to Main Transformer Connection

This is the primary and most critical IPB application in any thermal power plant. The IPB run connects the generator output terminal to the high-voltage side of the main step-up transformer.

Typical configuration:

```
Generator (20 kV / 600 MW)
    │
    ├── IPB main run ── Main Transformer (500 kV / 20 kV)
    │
    ├── Branch IPB ── Unit Auxiliary Transformer (UAT)
    │
    ├── Branch IPB ── Excitation Transformer
    │
    └── Branch IPB ── PT Cabinet / Lightning Arrester
```

### 2.2 Typical Electrical Parameters

| Parameter | Typical Value Range |
|-----------|--------------------|
| Generator voltage | 10.5 kV – 24 kV |
| Generator rated current | 3,000 A – 25,000 A |
| IPB rated current | 1,000 A – 35,000 A |
| Short-time withstand (2 s) | 50 kA – 315 kA |
| Peak withstand | 125 kA – 800 kA |
| Rated frequency | 50 Hz / 60 Hz |
| Protection degree | IP54 – IP65 |
| Enclosure temperature rise | < 30 K above ambient |

### 2.3 Generator Circuit Breaker Position

Two primary schemes exist for the generator circuit breaker (GCB):

**Scheme A — GCB on transformer side (most common in China)**
- IPB connects generator terminal to GCB, then GCB to transformer
- Allows generator to be isolated for maintenance while plant is operating
- Requires IPB branch sections on both sides of the breaker

**Scheme B — GCB on generator terminal side**
- IPB connects GCB to transformer only
- Generator must be de-energised to perform maintenance
- Simpler IPB layout, slightly lower cost

The choice of scheme affects IPB layout, civil works, and maintenance procedures. It should be confirmed early in the project design phase.

---

## 3. Auxiliary System Connections

![Neutral Grounding Cabinet](/images/wetown/ngc.png "Neutral Grounding Cabinet for IPB System")

### 3.1 Unit Auxiliary Transformer (UAT) Connection

The UAT supplies power to all auxiliary equipment within the generating unit — from mill motors and fan drives to the plant's internal lighting and control systems. The IPB branch to the UAT must accommodate:

- **Inrush current during transformer energisation** — up to 8–12× rated current for 0.1 s
- **Load rejection transients** — when the unit trips, the UAT must hold auxiliary loads while the unit is synchronising or shutting down
- **Mechanical layout coordination** — UAT is typically located at a different elevation than the generator, requiring IPB routing through civil structures

### 3.2 Excitation Transformer Connection

The excitation transformer feeds the generator's field excitation system. The IPB branch is typically short — often just one section with a flexible connection at the generator terminal. Key considerations:

- **Harmonic filtering** — if static excitation is used, harmonics from the thyristor converter may propagate into the IPB
- **Ground fault sensitivity** — excitation system ground faults must be detected without causing IPB protection to trip

### 3.3 PT and Lightning Arrester Connections

![PT & LA Cubicle](/images/wetown/PT & LA Cubicle.png "PT & LA Cubicle for IPB Protection")

Potential transformer (PT) and lightning arrester branches are short IPB sections that require:

- **Secondary wiring routing** — PT secondary cables must be routed to the protection relay cubicle
- **Coordinated surge protection** — lightning arrester rating must match the IPB and transformer BIL (basic impulse insulation level)

---

## 4. Civil Structure Coordination

IPB installation in a thermal power plant requires intensive civil structure coordination. This is one of the most common sources of interface risk in IPB projects.

### 4.1 Cable and Busbar Trench Layout

IPB typically runs along a dedicated cable and busbar trench (电缆母线沟) that must be coordinated with:

- **Excavation levels** — IPB support steel structures are anchored to concrete bases in the trench floor
- **Drainage** — trenches must be drained to prevent water accumulation around IPB supports
- **Adjacent cable routes** — control cables must be routed separately from power IPB to prevent electromagnetic interference

### 4.2 Support Steel Structures

IPB support structures are typically galvanised steel frames or lattice towers that:

- Support IPB at specified intervals (typically 3–6 m depending on short-circuit rating and seismic zone)
- Provide earthing connections for each IPB enclosure section
- Allow for thermal expansion (expansion joints every 20–30 m in outdoor runs)

Support structure drawings must be coordinated with the IPB supplier to ensure hole patterns, base plate dimensions, and anchor bolt specifications match.

### 4.3 Wall and Floor Penetrations

IPB passes through walls and floors at multiple points:

- Generator hall wall (generator to transformer yard)
- Transformer foundation penetration
- Switchgear building walls

Each penetration requires a **fire-rated penetration seal** and a **biologically sealed gland plate** to prevent moisture and small animals from entering the IPB enclosure.

---

## 5. Environmental and Site Conditions

### 5.1 Temperature and Climate

IPB for thermal power plants must be specified for the full range of ambient conditions at the site location:

| Climate | Design Temperature Range |
|---------|------------------------|
| Temperate | -25°C to +45°C |
| Hot-dry (e.g., Northwest China) | -30°C to +55°C |
| Tropical (e.g., Southeast Asia) | -10°C to +50°C |
| High altitude (>1,000 m) | Derate current rating per IEC 60815 |

For high-altitude sites, IPB current ratings must be derated because of reduced air density and cooling capacity. The supplier should confirm derating factors based on actual site elevation.

![Air Circulation Drying Unit](/images/wetown/ACDU.png "ACDU for IPB Enclosure Climate Control")

### 5.2 Pollution and Coastal Environments

In thermal power plants located in coastal areas or heavy industrial zones, pollution deposits on IPB insulation surfaces can reduce breakdown voltage. Countermeasures include:

- **Increased creepage distance** on insulator surfaces
- **RTV silicone coating** on composite insulators
- **Regular washing programmes** for outdoor insulator strings
- **IP65 enclosure rating** for outdoor runs in heavy pollution zones

### 5.3 Seismic Requirements

Power plants in seismic active zones (common in Southwest China and many Southeast Asian countries) require IPB designed to **IEEE 693** or equivalent seismic standards. Key requirements include:

- **Qualification testing** or analytical verification at the required seismic level
- **Flexible connections** at equipment interfaces to accommodate differential displacement
- **Support structure design** to resist seismic loads without collapse

---

## 6. Monitoring and Protection Systems

### 6.1 Temperature Monitoring

IPB temperature monitoring is increasingly standard on new power plant projects. Common systems include:

- **Embedded RTD sensors** on conductor surfaces at key locations (joints, terminations, centre of long spans)
- **Infrared window inspection** ports for periodic thermal imaging without de-energisation
- **Online monitoring systems** with DCS integration for continuous temperature logging and alarm generation

### 6.2 Pressure and Humidity Monitoring

For IPB with micro-positive pressure systems, continuous monitoring of:

- Enclosure internal pressure (relative to atmosphere)
- Relative humidity inside the enclosure
- Moisture dew point

allows operators to trigger drying systems before condensation forms on insulation surfaces.

### 6.3 Protection Coordination

IPB protection must coordinate with upstream and downstream protection devices:

| Protection Zone | Primary Protection | Backup Protection |
|---------------|-------------------|-------------------|
| Generator to GCB IPB | Generator differential relay | GCB breaker failure relay |
| GCB to transformer IPB | Busbar differential relay | Transformer backup relay |
| UAT branch | Overcurrent relay | -- |
| Excitation branch | Overcurrent relay | -- |

Protection relay settings must be coordinated with the IPB supplier to ensure thermal withstand limits are not exceeded during fault clearing times.

---

## 7. Pre-Commissioning Checks

Before energisation, IPB systems require a comprehensive pre-commissioning test sequence:

1. **Visual inspection** — verify all bolted joints are correctly torqued, all earth connections are made, no foreign objects in enclosures
2. **Resistance measurement** — measure and record contact resistance of every bolted joint (typically < 20 μΩ per joint)
3. **Insulation resistance test** — phase-to-phase and phase-to-earth at 1 kV DC (minimum 1,000 MΩ for clean, dry IPB)
4. **Voltage withstand** — 2.5× rated voltage AC for 1 minute (between phases and phase to earth)
5. **Partial discharge test** — if specified, PD levels should be < 10 pC at rated voltage
6. **Expansion joint function test** — verify expansion joints can move freely within design range
7. **Earthing continuity test** — verify every enclosure section is properly bonded to earth bar
8. **Monitoring system functional test** — verify all sensors, transmitters, and DCS interfaces are operational

---

## 8. Common Design and Interface Issues

### 8.1 Information Required from the IPB Supplier

To complete the civil and electrical design, the plant designer needs from the IPB supplier:

- **IPB general arrangement drawing** (plan and elevation views)
- **Support point locations and loadings** (for civil structure design)
- **Junction and termination details** (for cable and secondary system design)
- **Earthing layout drawing** (for earth mat design)
- **Foundation load data** (for transformer and equipment foundation design)
- **Fire barrier specifications** (for penetration design)

### 8.2 Interface Risk Areas

The most common sources of delay and rework in IPB projects:

- **Civil-Busbars interface** — incorrect support anchor bolt locations or levels
- **Cable-Busbars interface** — gland plate dimensions not matching cable termination requirements
- **Transformer-Busbars interface** — transformer terminal direction or elevation not matching IPB termination design
- **Secondary-Busbars interface** — CT (current transformer) locations in IPB branch not matching protection relay design

Early confirmation of these interfaces in the design phase significantly reduces project risk.

---

## Related Articles

- [Isolated Phase Busbar (IPB): Complete Technical Guide](/blog/isolated-phase-busbar-ipb-guide/) — Comprehensive IPB engineering reference
- [IPB vs NSPB: What Is the Difference?](/blog/ipb-vs-nspb/) — Comparison of the two major enclosed busbar technologies
- [How to Choose the Right Busbar System for a Power Plant](/blog/how-to-choose-the-right-busbar-system-for-a-power-plant/) — Plant-level selection methodology
- [IPB vs NSPB: What Is the Difference?](/blog/ipb-vs-nspb/) — Comparison of the two major enclosed busbar technologies
