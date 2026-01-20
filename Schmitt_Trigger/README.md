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
