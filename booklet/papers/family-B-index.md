# Family B — Multi-axis curved-layer field / deformation

Canonical paper cards for robot / 5-axis curved layers built from scalar, geodesic, stress, quaternion-deformation, or neural fields.
Cards: `/home/box/fnps-research/papers/cards/`. Template: `CARD_TEMPLATE.md`. Sources: `held-papers.json`, `paper-01.txt`.

| ID | Paper card | When to use |
|---:|---|---|
| 016 | [Geodesic distance field curved-layer decomposition (2020)](../../papers/cards/016-geodesic-distance-field-curved-layer-decomposition.md) | Robot or 5-axis cell; support-free volume where layers should follow geodesic distance from a base/seed. |
| 018 | [INF-3DP (2025)](../../papers/cards/018-inf-3dp.md) | Multi-axis volumes where both a guidance field for layers and a motion field for the nozzle should be implicit neural. |
| 020 | [Implicit neural field process planning (2026, accepted CAD)](../../papers/cards/020-implicit-neural-field-process-planning.md) | CAD-integrated process planning where both layers and in-layer paths are SIREN fields. |
| 026 | [Multi-axis support-free printing with lattice infill (2020)](../../papers/cards/026-multi-axis-support-free-printing-with-lattice-infill.md) | Support-free multi-axis print where the *infill itself* is a self-supporting lattice, not only solid curved shells. |
| 029 | [Neural Slicer (2024)](../../papers/cards/029-neural-slicer.md) | Multi-axis product roadmap wants learned / differentiable deformation fields instead of hand-crafted geodesic or stress PDEs. |
| 042 | [Reinforced FDM (2020)](../../papers/cards/042-reinforced-fdm.md) | Strength-critical part on a multi-axis cell: bead / layer direction should follow principal stress. |
| 045 | [S3-Slicer (2022)](../../papers/cards/045-s3-slicer.md) | Multi-axis job must jointly hit support-free, strength, and surface-quality goals (S3 = three objectives). |
| 051 | [Support generation for curved layers (2023)](../../papers/cards/051-support-generation-curved-layers.md) | Multi-axis curved layers still leave local overhangs that fail the Part F local-overhang gate. |
| 066 | [Support-Free Volume Printing (Dai 2018)](../../papers/cards/066-support-free-volume-printing-dai.md) | Robot or 5-axis cell must print a solid volume without sacrificial supports. |
| 068 | [Topological awareness, collision-free curved layers (2024)](../../papers/cards/068-topological-awareness-curved-layers.md) | Curved layers already exist (geodesic / deformation / neural) but tunnels and branches break naive bottom-up order. |
| 069 | [Curved Layer Process Planning (Xu 2019)](../../papers/cards/069-curved-layer-process-planning-xu.md) | Multi-axis (robot / 5-axis) job needs curved layers that follow surface geodesics rather than a voxel growth front. |

## Chaining (quick)

- **G → B:** self-support TO (#48/#47/#50) before a field.
- **B → E:** Reinforced / geodesic / neural layers → continuous-fiber packing (#15/#10/#52).
- **B → D:** TCP layers → singularity-aware / FRIK / env-aware motion (#49/#64/#63).
- **B → #51:** residual local overhang after field/deformation still needs tree supports.
- **Do not:** escalate to B on Cartesian-only hardware when family A clearance cone still holds.

## Inventory flags

- **#51** — missing DOI/arXiv link in `held-papers.json` (`Link: —`).
- **Code (Part D):** Reinforced FDM → `github.com/GuoxinFang/ReinforcedFDM`; S3-Slicer → `github.com/zhangty019/S3_DeformFDM`; geodesic tools → geometry-central.
- **Also arXiv:** #18 → 2509.05345; #20 → 2511.17578v2.
