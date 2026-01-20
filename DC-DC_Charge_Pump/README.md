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

---

## Working Principle

The DC–DC charge pump operates by transferring charge between capacitors using a clock-driven switching action.

During the high phase of the clock signal, the capacitor is charged to the input voltage.  
During the low phase, the stored charge is transferred through the diode to the output capacitor, increasing the output voltage.

Schottky diodes are used to reduce forward voltage drop and improve efficiency.

---

## Design Relation (Ideal Case)

For a single-stage charge pump:

Vout ≈ Vin − 2VD

Where:
- Vin is the input DC voltage
- VD is the diode forward voltage

In practical conditions, output voltage reduces due to diode losses and load current.
