# Changelog

## [Unreleased]
C3 decreased for shorter dead time
R15 increased to compensate C3 
R26 increased to reduce slope compensation
R31 added as alternative for slope compensation
C4 updated to 1 nF
C20, C21 and R20 updated (slower compensation)
R3 increased (gain = 1 on error amp.)
C2 not fitted (secondary side compensation only)
R8 package increased to 1206
D23 removed
Default optocoupler supply swapped R29->R28
R32 added to facilitate compensation tests
Added snubber accross D4
Enlarged C24 and C27 footprint
Silk typos fixed (HV+/HV-)
Fixed R9 footprint and added alternative footprint (R35)

wrong footprint for shunt
add snubber (pri)



## [2.0.0] - 2026-02-07

### Added R29 as feed-forward option

Isolated primary ("LV") and secondary ("HV") sides
Updated reverse polarity protection (based on P-channel MOSFET)
Added dedicated connectors for supply input
Replaced C6 (100 uF elco -> 4.7 uF + 100 nF MLCCs)
Added C25 to support testing
Replaced packages (U1: DIP-8 -> SOIC-8; U21: TO-92 -> SOT-23)
Replaced U20 (SH816 -> TCMT1108)
Replaced Q20 (2N2222 -> BC817)
Reworked slope compensation
Updated F1 footprint and 3D model
Added part number to D4
Updated Mod20 decoupling and added R30 as load
Added testpoints
Added clearance rules


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

[Unreleased]: https://github.com/FLRHW/Isolated_12to450V/compare/2.0.0...HEAD

[2.0.0]: https://github.com/FLRHW/Isolated_12to450V/compare/1.0.0...2.0.0

[1.0.0]: https://github.com/FLRHW/Isolated_12to450V/compare/f8c9afb6a11647257dfa5ab046e95b1ec53fcfd7...1.0.0
