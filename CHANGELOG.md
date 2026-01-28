# Changelog

## [Unreleased]

### Updated UC3845 symbol
Added R29 as feed-forward option
Updated UC3845 symbol
Isolated primary ("LV") and secondary ("HV") sides
Reorganised schematic for readability
Replaced reverse polarity protection circuit by one based on a P-channel MOSFET
Added dedicated screw terminals for input power and reused existing 4-way connector for the output
Replaced C6 from 100 uF elco to 4.7 uF + 100 nF MLCCs
Reserved footprint for C25 to test a different compensation circuit
Replaced U1 package from DIP-8 to SOIC-8
Replaced U21 package from TO-92 to SOT-23
Replaced U20 from SH816 to TCMT1108
Replaced Q20 from 2N2222 to BC817
Reworked slope compensation / ramp generation
Updated fuse clip footprint
Added part number to D4


To do:
- Identify suitable P-MOS

## [1.0.0] - 2026-01-24

### Cloned non-isolated design revision 1.1.0 as a working base.
Updated R10 and R11 to 240 kΩ (cloned design incorrectly used 140 kΩ).
Updated U1 to UC3845 (cloned design incorrectly used UC3843).
Reworked feedback loop to include opto-coupler while keeping the same reference on both sides to facilitate testing / reuse of original board.
Added two options of slope compensation / ramp injection (from U1 RT_CT pin and from U1 OUTPUT pin).
Adjusted R2 to 10 kΩ, R3 to 5 kΩ and C2 to 1 nF to improve behaviour (output swaps from bursts to 0 % duty periodically).
Added soft-start (D21, R27 and C23).
Increased C5 to 100 nF.
Adjusted C4 to 1.5 nF and R6 to 1 kΩ (similar time constant) to facilitate ramp injection.
Updated parts placement where suitable to reuse existing layout and added an auxiliary perf-board to accomodate the new parts.

[Unreleased]: https://github.com/FLRHW/Isolated_12to450V/compare/1.0.0...HEAD

[1.0.0]: https://github.com/FLRHW/Isolated_12to450V/compare/f8c9afb6a11647257dfa5ab046e95b1ec53fcfd7...1.0.0
