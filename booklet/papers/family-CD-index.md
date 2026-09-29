# Family C–D paper-card index

Per-paper cards for multi-directional decomposition / shells / hardware (**C**) and motion planning / kinematics / robots (**D**).
Cards: `/home/box/fnps-research/papers/cards/`. Template: `CARD_TEMPLATE.md`. Sources: `held-papers.json`, `paper-01.txt`.

When duplicate slug files exist, this index links the longer (richer) card.

## Family C — Multi-directional decomposition, shells, hardware

| # | Paper | When to use |
| --- | --- | --- |
| 43 | [`043-robofdm.md`](../../papers/cards/043-robofdm.md)<br>RoboFDM (2017) | Use when the part has large overhangs that a stock 3-axis clearance cone cannot cover, and you prefer cutting the volume into support-free planar chunks over… |
| 70 | [`070-near-support-free-multidir.md`](../../papers/cards/070-near-support-free-multidir.md)<br>Near support-free multi-directional printing (2019) | Use when RoboFDM-style multi-directional printing is desired but cutting planes and fabrication order must be optimized automatically for near-minimal overhang… |
| 28 | [`028-metu-spiral-tnb.md`](../../papers/cards/028-metu-spiral-tnb.md)<br>Multi-axis spiral parts without supports (METU 2021) | Use when the part follows a helical / spiral guide (springs, screws, spiral ornaments, ducted spirals) and multi-axis hardware can keep planar slices roughly… |
| 37 | [`037-romex-conical.md`](../../papers/cards/037-romex-conical.md)<br>RoMEX non-planar robotic path planning (2023) | Use when the part suits a conical deposition strategy — stacked 45° conical shell layers wrapping a core — on a robotic MEX cell, and you want hardware-native… |
| 73 | [`073-acap.md`](../../papers/cards/073-acap.md)<br>ACAP (2023) | Use for thin shell / surface models (architectural skins, ceramic vessels, open shells) where transfer moves destroy surface quality and stability — especially… |
| 30 | [`030-double-shells.md`](../../papers/cards/030-double-shells.md)<br>Non-planar printing of double shells (2025) | Use for architectural thin double-shell structures (façade panels, concrete-casting molds, pavilion skins) fabricated on multi-axis robotic FDM. Prefer when… |
| 33 | [`033-open5x.md`](../../papers/cards/033-open5x.md)<br>Open5x (2022) | Use when upgrading a desktop 3-axis FFF printer with a rotary-plus-tilt bed (U/V) for accessible conformal / 3+2 printing, and the workflow should stay inside… |
| 1 | [`001-conformal-antennas.md`](../../papers/cards/001-conformal-antennas.md)<br>5-axis multi-material conformal antennas (2025) | Use when fabricating functional conformal RF antennas (patch, UWB, curved traces) that need conductive + dielectric beads on a curved substrate, on an… |

## Family D — Motion planning, kinematics, robots

| # | Paper | When to use |
| --- | --- | --- |
| 49 | [`049-singularity-aware-motion.md`](../../papers/cards/049-singularity-aware-motion.md)<br>Singularity-aware motion planning (2021) | Downstream of B/C/E curved or multi-directional toolpaths on a 5-axis Cartesian printer (table-table, head-head, or head-table) when tool vectors pass near the… |
| 64 | [`064-frik.md`](../../papers/cards/064-frik.md)<br>FRIK: fast redundant IK (2025) | Six-axis industrial arms executing AM / cold-spray / WAAM / welding toolpaths where the tool axis is rotationally symmetric (free roll about the nozzle) —… |
| 63 | [`063-env-aware-path-gen.md`](../../papers/cards/063-env-aware-path-gen.md)<br>Environment-aware path generation for robotic AM (2026) | On-site / expeditionary / outdoor robotic construction where obstacles are known only at print time — offline CAD→slice G-code cannot see the workspace. |
| 39 | [`039-printing-while-moving.md`](../../papers/cards/039-printing-while-moving.md)<br>Printing-while-moving (2018) | Large-scale concrete / construction AM where the structure exceeds arm reach and stop-and-print mobile bases would force seams, size limits, or escape-path… |
| 54 | [`054-cooperative-robotics-review.md`](../../papers/cards/054-cooperative-robotics-review.md)<br>Cooperative robotics in AM (review 2024) | Scoping a multi-arm / C-RAM product: high-overlap (multi-material, multi-resolution, cooperative sensing) vs low-overlap (large-scale homogeneous tooling). |
| 38 | [`038-indexed-rotary-grbl.md`](../../papers/cards/038-indexed-rotary-grbl.md)<br>Indexed rotary post-processor for GRBL (2025) | Low-cost GRBL desktop CNC (education, makerspace, prototyping) that has a spare axis channel and a mechanical rotary chuck but vanilla GRBL has no true… |

## Chaining (quick)

- **C → A:** planar fill inside each decomposed chunk / patch.
- **C → E:** fiber along shell geodesics after ACAP / double-shell patches.
- **C → D:** robot / 5-axis trajectories between orientations and patches.
- **B/C/E → D:** singularity-aware poses, FRIK, env-aware links, then TOPP-RA timing.
- **D hardware ladder:** Open5x / indexed GRBL (#33/#38) → conical RoMEX (#37) → RoboFDM / multi-dir (#43/#70) → mobile / multi-robot (#39/#54).

## Missing registry links

- #28 METU spiral TNB — no link in `held-papers.json`
- #33 Open5x — no link in registry (public CHI / GitHub noted on card)
- #37 RoMEX conical — no link in `held-papers.json`
