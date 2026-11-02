# Circuits simulations in LTspice

## Project overview

This repository is a library of LTspice schematics for power conversion, analog building blocks, filters, oscillators, and small-signal circuits. Each circuit is an `.asc` file, so it opens and runs directly in LTspice.

Schematics are grouped by function. Power folders cover rectifiers, inverters, DC-DC converters, transformers, and protection. Analog folders cover amplifiers, comparators, current sources, and regulators. Signal folders cover filters, oscillators, modulators, triggers, and basic transistor examples.

## How to use

1. Install [LTspice](https://www.analog.com/en/resources/design-tools-and-calculators/ltspice-simulator.html).
2. Open any `.asc` file from the folders below.
3. Run the simulation from the LTspice toolbar.

A few folders include a Python script next to the schematic. Those scripts calculate component values that are then entered in LTspice.

## Examples

### Common-emitter BJT
![Common-emitter BJT configuration](https://user-images.githubusercontent.com/13961654/53668789-30dada00-3c75-11e9-9655-df0a41e2482b.png)

### Sawtooth oscillator
![Sawtooth oscillator](https://user-images.githubusercontent.com/13961654/53668794-320c0700-3c75-11e9-8d3c-cfd66af27392.png)

### Three-phase full-bridge inverter
![Three-phase full-bridge inverter with wye and delta loads](https://user-images.githubusercontent.com/13961654/53668796-33d5ca80-3c75-11e9-9dc6-d9cf26519e03.png)

## Contents

### Power conversion

| Folder | Circuits |
| --- | --- |
| `AC-DC and DC-AC converters` | Single-phase and three-phase rectifiers, half-bridge and full-bridge inverters, and a full-bridge DC-DC stage |
| `DCDC converters` | Buck and boost converters |
| `Transformer` | Transformer circuits |
| `Power-lines` | Power-line examples |
| `Voltage-elevator-circuits` | Voltage step-up circuits |
| `Soft-starters` | Soft-start circuit |
| `Pwm` | PWM example |
| `Overvoltage protection circuits` | Overvoltage protection |

### Amplifiers, sources, and control

| Folder | Circuits |
| --- | --- |
| `Amplifiers` | Common-emitter, emitter-follower, differential, instrumentation, and push-pull stages |
| `Input stages` | Professional input stage |
| `Comparator circuits` | Window comparators and Schmitt triggers, with and without hysteresis |
| `Current-mirrors` | BJT current mirror and current source |
| `Current limiting circuits` | Simple BJT current limiters |
| `Sources and regulators` | Sources and regulator circuits |
| `Controller-control-systems` | Bang-bang control, a closed-loop buck converter, and a PD controller |
| `Loads` | Load examples |

### Filters, oscillators, and signals

| Folder | Circuits |
| --- | --- |
| `Filters` | RC, RL, and RLC low-pass, high-pass, band-pass, and notch filters, including step response |
| `Oscillators` | 555 timer, astable, phase-shift, Wien, Royer ZVS, and related oscillators |
| `Lossless-transmission-line` | DC transient and pulse behavior of a lossless line |
| `Signal processing` | Signal-processing circuits |
| `Trigger circuits` | Trigger circuits |
| `Zero-crossing-detectors` | Zero-crossing detectors |
| `Logic-circuits` | Logic examples |
| `AM-modulator-circuits` | BJT and JFET AM modulators |
| `ASK-modulator-transceiver` | ASK modulation circuits |
| `Mixer-circuits` | Mixer circuit |
| `RF-generators` | RF generator |

### Device behavior and checks

| Folder | Circuits |
| --- | --- |
| `Basics` | DC sweep, initial conditions, biasing, and transistor beta |
| `Monte-Carlo-simulations` | Monte Carlo runs |
| `Worst-case-scenario-simulation` | Worst-case runs |
| `Temperature-variation-simulation` | Temperature sweeps |
| `Tested-circuits` | Circuits checked against a built or measured case |
| `Others` | Additional one-off circuits |
| `Miscellaneous` | Circuits that do not fit the groups above |
