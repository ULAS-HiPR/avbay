# Avbay current system

Updated 22 November 2026. Decisions live in [decisions.md](decisions.md); this file states
what is true now. Nothing is designed, built or flown yet.

Owner: Alex. Helpers: Rory. Next milestone: Bay mockup with mechanical; access panel requirements captured by 14 Dec.

Seeded from the [Notion brief](https://app.notion.com/p/41ecc5f72fe281538883e08f6f233f37) and [access panel brief](https://app.notion.com/p/41ecc5f72fe281b7bb76e33f9f001313) and from Ogma2's decisions as they stood on
22 November. Where they disagree, Ogma2's decisions win.

## Purpose

Two jobs, one owner. **Av-bay integration:** with mechanical, fit the electronics into the vehicle: mounts, vents, antennas, packs, the CATS Vega, and the wiring between bays. **Access panel and harness:** put everything the pad crew touches on one panel, low on the airframe and opposite the rail ([D-21Nov.5](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md)), and build every harness to a drawing.

## Must demonstrate

- A bay mockup that takes Burrito and Churro, the CATS Vega and the packs.
- A barometer vent; antennas inside a 360° RF window at least two calibres long (about 305 mm at 6 in), not carbon fibre, each at its midpoint (LV-0780–0820).
- The two recovery chains sharing no power, wiring or vent.
- Every switch and plug reached from the ground with the rocket vertical on a rail, without a ladder; every pack charging through the umbilical. Mockup first, then the vehicle.
- A tug test and a continuity check on every harness. The panel secured for flight.

## Interfaces

Set by Ogma2's decisions unless marked proposed. Changing one needs the other
owner's agreement and a row in both repositories.

| With | What | Ogma2 decision |
| --- | --- | --- |
| Burrito and Churro | Their mounting: Burrito bolted edge to edge to Churro; every board 80 mm wide. Each connector sits at the end its harness leaves by. | [D-21Nov.6](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md), [D-21Nov.24](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md) |
| Burrito | Two SMA antenna plugs, labelled. The pyro leads to the recovery bay. Recovery and staging arm switches to J6101 (2-way) and J6102 (3-way). Enable loop J103: Molex Micro-Fit 3.0, single row, two circuits. | [D-22Nov.18](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md) |
| Churro | The umbilical: required, carries charging too, survives hot-plugging; a pull-away at the skin that releases at Go. Enable loops J103 and J104. The packs stay in the vehicle and charge through the umbilical; no battery hatch. | [D-20Nov.1](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md), [D-21Nov.3](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md), [D-2Nov.7](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md) |
| Fajita, Salsa | Bus 1 to Fajita and bus 2 to the active module, Harwin Gecko, point to point. Salsa's arm key on the panel. | [D-18Nov.4](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md) |
| Panel | One USB-C per programmable board (Burrito, Fajita, Salsa), beside the umbilical plug; USB-C stays at the av-bay, nothing flashed on the rail. Also the CATS Vega's switch. | [D-19Nov.9](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md), [D-21Nov.4](https://github.com/ULAS-HiPR/Ogma2/blob/main/decisions.md) |

## Also known

- Decided (Notion brief, citing D-19Nov.4): keyed, shrouded, positive-lock connectors; a label on every switch, plug and port; the sounder beeps continuity and state at arming.
- The access rule asks for physical reach of hand-operated switches and connectors, and of the batteries (LV-0260–0280, 0310). Switches and plugs can mount straight on the skin, so no hatch is needed. The USB-C ports are our choice, not EuRoC's.

## External rules

LV-0780–0820 (RF window); LV-0240 (each recovery chain on its own battery); LV-0260–0280, 0310, 0540–0550 (access); LV-0480–0500 (wiring: cable management, secure connections, cryogenic-rated insulation near the N₂O); LV-0530 (energetics safed until in launch position); Appendix C (a charging bus with connectors at every joint); Appendix E1 (a hand-operated disconnect in the valves' power, a "should").

## Parts one person can own

1. The bay mockup: mounts, packs, CATS Vega, vents
2. Antennas and the RF window
3. The access panel: switches, plugs, labels, its position and height
4. The umbilical and the charging bus across every joint
5. Harness drawings, tug and continuity tests

## Timeline

| Milestone | Date |
| --- | --- |
| Requirements captured | 14 December 2026 |
| Schematics reviewed | 28 December 2026 |
| PCBs laid out and ordered | 11 January 2027 |
| Boards in hand | 1 February 2027 |
| Testing, firmware and integration | from 1 February 2027 |
| All electronics on one table | 3 weeks before the integrated vehicle |

From the [Electronics page](https://app.notion.com/p/3c8cc5f72fe28092aaf7dc3baacb4f67)'s avionics timeline.

## State

Repository created 22 November 2026. No requirements, schematic, layout or
firmware yet. Open questions are in [decisions.md](decisions.md#open).
