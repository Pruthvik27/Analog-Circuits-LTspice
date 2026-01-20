## Schmitt Trigger

Objective:
To convert a noisy analog signal into a clean digital output.

Key Concepts:
- Positive feedback
- Upper and lower threshold voltages
- Hysteresis

Files (to be added):
- schmitt_trigger.asc
- schematic.png
- hysteresis_waveform.png

Tool Used:
- LTspice

### Components Used
- Operational amplifier: OP07
- Resistors: 25 kΩ, 100 Ω
- Input source: SINE(0 5 1k)
- DC supplies: +12 V (2×), 3 V reference
- Transient analysis: .tran 70m

---

---

## Working Principle

The Schmitt Trigger is a comparator circuit with **positive feedback**, which introduces hysteresis into the switching behavior.

When the input voltage rises above the **upper threshold voltage**, the output switches to the high saturation level.  
When the input voltage falls below the **lower threshold voltage**, the output switches to the low saturation level.

Because two different threshold voltages exist, small noise or slow variations at the input do not cause false switching.  
This makes the Schmitt Trigger useful for signal conditioning and noise immunity.

---

## Design Equations

Let:
- R1 = feedback resistor
- R3 = reference resistor
- Vref = reference voltage
- Vout = output saturation voltage

### Upper Threshold Voltage (VUT)
VUT = Vref + (R3 / R1) × Vout

### Lower Threshold Voltage (VLT)
VLT = Vref − (R3 / R1) × Vout

---

### Hysteresis Width
Hysteresis = VUT − VLT

The amount of hysteresis depends on the resistor ratio and the output voltage levels.


Where:
- Av is the closed-loop gain of the op-amp

If gain is less than 3, oscillations die out.  
If gain is too high, waveform distortion occurs.
