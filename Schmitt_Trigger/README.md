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

## Working Principle

The Wien Bridge Oscillator generates a sinusoidal output using a frequency-selective RC bridge network combined with an operational amplifier.

The RC network provides **positive feedback** at a specific frequency, while the resistor network around the op-amp provides **negative feedback** to control the gain.

At the oscillation frequency:
- Phase shift through the RC network is 0°
- Loop gain becomes unity
- Sustained oscillations are produced

The op-amp supplies the required gain, and the RC bridge determines the frequency of oscillation.

---

## Design Equations

### Oscillation Frequency
For equal resistor and capacitor values:

f₀ = 1 / (2πRC)

Where:
- R = Resistance in the Wien bridge network
- C = Capacitance in the Wien bridge network

---

### Gain Condition for Oscillation

To sustain oscillations:

Av ≥ 3

Where:
- Av is the closed-loop gain of the op-amp

If gain is less than 3, oscillations die out.  
If gain is too high, waveform distortion occurs.
