## DC–DC Charge Pump

Objective:
To design and simulate a DC–DC charge pump using LTspice.

Description:
This circuit boosts DC voltage using a capacitor–diode charge transfer mechanism.

Files (to be added):
- charge_pump.asc
- schematic.png
- output_waveform.png

Tool Used:
- LTspice

### Components Used
- Pulse voltage source (clock): PULSE(0 5 0 10n 10n 0.5u 1u)
- DC voltage source: 1 V
- Diodes: 1N5818 (2×)
- Capacitors: 1 µF (2×)
- Transient analysis: .tran 4m

