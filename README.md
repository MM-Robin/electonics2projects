<div align="center">

# Electronics Lab Projects

**Analog Circuit Design · SPICE Simulation · Semiconductor Devices**

[![LTspice](https://img.shields.io/badge/Tool-LTspice-A4373A?style=flat-square)](https://www.analog.com/en/resources/design-tools-and-calculators/ltspice-simulator.html)
[![Language](https://img.shields.io/badge/Simulation-SPICE-5C2D91?style=flat-square)]()
[![Domain](https://img.shields.io/badge/Domain-Analog%20Electronics-0078D4?style=flat-square)]()
[![HAW Hamburg](https://img.shields.io/badge/HAW-Hamburg-004F9F?style=flat-square)]()

</div>

---

## Overview

This repository contains **LTspice circuit simulation projects** from the **Electronics Lab** course at **HAW Hamburg**. The experiments cover fundamental analog semiconductor devices and circuits — from MOSFET characterization and BJT amplifier design to operational amplifiers and 555 timer applications.

Each `.asc` file is an LTspice schematic ready to simulate.

---

## Repository Structure

```
electonics2projects/
│
├── MOSFET/                        # MOSFET characterization & applications
│   ├── MOSFET.asc                 # MOSFET Id/Vgs curves, threshold voltage, transconductance
│   └── MOSFETasSwitchAndAmplifier.asc   # MOSFET as switch and single-ended amplifier
│
├── BJT_Transistor/                # Bipolar Junction Transistor (BJT) circuits
│   ├── transistorCkt.asc          # BC546A output & transfer characteristics
│   └── CommonEmitterCircuit.asc   # Common emitter amplifier — gain, Rin, Rout
│
├── Amplifiers/                    # Operational & differential amplifiers
│   ├── OperationalAmplifier.asc   # Op-amp input/output characteristics
│   └── DifferentialAmplifier.asc  # Differential amplifier — CMRR & optimization
│
└── Timer555/                      # NE555 timer circuit configurations
    ├── Timer555ForAstableOperation.asc    # Astable mode — free-running oscillator
    └── Timer555ForMonostableOperation.asc # Monostable mode — one-shot pulse
```

---

## Experiments

### MOSFET — Characterization & Applications

| File | Description |
|---|---|
| `MOSFET.asc` | Sweeps gate voltage to plot Id/Vgs curves. Extracts threshold voltage (Vth) and transconductance coefficient (k). Verifies current mirror behavior (I1 = I2). |
| `MOSFETasSwitchAndAmplifier.asc` | Demonstrates MOSFET operating in switch and amplifier regions. Defines input/output characteristics for single-ended amplifier configuration. |

**Concepts:** Transfer characteristics · Threshold voltage · Transconductance · Current mirror · Saturation vs. triode region

---

### BJT Transistor — BC546A

| File | Description |
|---|---|
| `transistorCkt.asc` | Plots output and transfer characteristics of BC546A NPN transistor. Graphically determines transconductance at a defined operating point. |
| `CommonEmitterCircuit.asc` | Common emitter amplifier. Measures DC operating point, AC voltage gain, and input/output resistance using the half-voltage method. |

**Concepts:** Ic/Vce output characteristics · Transfer curve · Q-point biasing · AC gain · Half-voltage resistance measurement

---

### Amplifiers — Op-Amp & Differential

| File | Description |
|---|---|
| `OperationalAmplifier.asc` | Analyzes op-amp input/output behavior. Characterizes gain, bandwidth, and operating limits. |
| `DifferentialAmplifier.asc` | Implements a differential amplifier from literature specifications. Investigates CMRR and circuit optimization techniques. |

**Concepts:** Open-loop vs. closed-loop gain · CMRR · Differential vs. common-mode signals · Circuit optimization

---

### NE555 Timer — Astable & Monostable

| File | Description |
|---|---|
| `Timer555ForAstableOperation.asc` | Free-running oscillator configuration. Frequency and duty cycle set by R/C network. |
| `Timer555ForMonostableOperation.asc` | One-shot pulse generator. Pulse width determined by R/C time constant. |

**Concepts:** RC time constant · Duty cycle · Trigger/threshold behavior · Oscilloscope waveform analysis

---

## Tools

| Tool | Purpose |
|---|---|
| **LTspice** | Schematic entry & SPICE simulation (`.asc` files) |
| **Oscilloscope** | Hardware waveform measurement and validation |
| **Multimeter** | DC operating point verification |

### Running a Simulation

1. Open any `.asc` file in **LTspice**
2. Press **Run** (F5) to start the SPICE simulation
3. Probe signals by clicking on nets or components
4. Use `.op`, `.dc`, `.ac`, or `.tran` directives already configured in each schematic

---

## Author

<div align="center">

**Mainuddin Monsur Robin**
*M.Sc. Information and Communication Engineering — HAW Hamburg*

[![GitHub](https://img.shields.io/badge/GitHub-MM--Robin-181717?style=flat-square&logo=github)](https://github.com/MM-Robin)

</div>
