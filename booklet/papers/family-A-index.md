# Family A — 3-axis / slightly non-planar FFF

Canonical paper cards for stock 3-axis or mildly tilted FFF workflows.

| ID | Paper card | When to use |
|---:|---|---|
| 004 | [Ahlers MSc thesis (2018)](../../papers/cards/004-ahlers-msc-2018.md) | Use for cone-safe cosmetic or mild freeform top skins on stock 3-axis FFF, especially after adaptive planar thickness. |
| 005 | [Ahlers CASE (2019)](../../papers/cards/005-ahlers-case-2019.md) | Use when a citable collision-cone gate is needed for cone-safe non-planar top patches on 3-axis FFF. |
| 006 | [Ahlers colloquium slides (2018)](../../papers/cards/006-ahlers-colloquium-slides-2018.md) | Use as an internal design/onboarding reference for the Ahlers lift-and-project skin pipeline, not as the primary implementation source. |
| 007 | [Anti-aliasing for fused filament deposition (Song et al. 2017)](../../papers/cards/007-anti-aliasing-for-fused-filament-deposition.md) | Use for fast cosmetic top improvement on stock 3-axis FFF via ZAA-style vertical vertex snapping. |
| 012 | [Curved Layer Based Process Planning (2017)](../../papers/cards/012-curved-layer-based-process-planning-2017.md) | Keep as an inventory alias only; its registry content is a duplicate of #7, so do not offer it as a distinct method. |
| 013 | [CurviSlicer (2019)](../../papers/cards/013-curvislicer-2019.md) | Use for mild whole-part curvature on stock 3-axis when local skin snaps are insufficient but a volume warp remains feasible. |
| 032 | [Modeling of non-planar slicer for MEX (2024)](../../papers/cards/032-modeling-of-non-planar-slicer-for-mex-2024.md) | Use for a planar structural core plus a cone-safe non-planar outer shell without warping the entire volume. |
| 041 | [QuickCurve (2024)](../../papers/cards/041-quickcurve-2024.md) | Use for a single slope-clamped height-field top or cover with oriented phasor patterning on 3-axis. |
| 056 | [Triple Z-axis FFF (2025)](../../papers/cards/056-triple-z-axis-fff-2025.md) | Use on RatRig-class Triple-Z hardware when mild bed tilt up to about 30° bridges stock 3-axis and fuller multi-axis motion. |
| 065 | [AtomSlicer (2026)](../../papers/cards/065-atomslicer-2026.md) | Use for dense field-aligned constant-thickness layers and continuous stripe fill on 3-axis or Triple-Z machines. |
| 067 | [Atomizer (2025)](../../papers/cards/067-atomizer-2025.md) | Use as a layer-free atom-frame ordering front-end when support/access cones make a global planar stack too rigid. |
| 071 | [Double QuickCurve (2025)](../../papers/cards/071-double-quickcurve-2025.md) | Use when both top and bottom surfaces need optimized height fields with interpolated mild-curved layers on 3-axis. |

**Inventory note:** #12 is an inventory duplicate of #7; prefer #7 for implementation and citation.
