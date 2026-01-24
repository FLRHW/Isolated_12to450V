# Changelog

## [Unreleased]

### Change description

Cloned non-isolated design revision 1.1.0 as a working base.
Updated R10 and R11 to 240 kΩ (cloned design incorrectly used 140 kΩ).
Updated U1 to UC3845 (cloned design incorrectly used UC3843).
Reworked feedback loop to include opto-coupler while keeping the same reference on both sides to facilitate testing / reuse of original board.
Added two options of slope compensation / ramp injection (from U1 RT_CT pin and from U1 OUTPUT pin).
Adjusted R2 to 10 kΩ, R3 to 5 kΩ and C2 to 1 nF to improve behaviour (output swaps from bursts to 0 % duty periodically).
Added soft-start (D21, R27 and C23).
Increased C5 to 100 nF.
Adjusted C4 to 1.5 nF and R6 to 1 kΩ (similar time constant) to facilitate ramp injection.
Updated parts placement where suitable to reuse existing layout and added an auxiliary perf-board to accomodate the new parts.