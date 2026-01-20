## Wien Bridge Oscillator

Objective:
To generate a low-distortion sine wave using a Wien bridge network.

Key Points:
- Frequency set by RC network
- Gain ≥ 3 for oscillation

Files (to be added):
- wien_bridge.asc
- schematic.png
- sine_output.png

Tool Used:
- LTspice

### Components Used
- Operational amplifier: OP07
- Resistors: 4.9 kΩ, 10 kΩ, 7.5 kΩ (2×)
- Capacitors: 10 nF (2×)
- Dual power supply: +5 V, −5 V
- Transient analysis: .tran 0.01

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
