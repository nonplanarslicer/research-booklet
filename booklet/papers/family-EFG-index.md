# Family E–F–G (+ VPP + Process) paper-card index

Per-paper cards for continuous fiber (**E**), general toolpath / planar-adaptive / mesh formats (**F**), topology / DfAM (**G**), plus assigned **VPP** and **Process** entries.
Cards: `/home/box/fnps-research/papers/cards/`. Template: `CARD_TEMPLATE.md`. Sources: `held-papers.json`, `paper-01.txt`.

One card file per ID. Relative links from this booklet path.

## E — Continuous fiber / anisotropy

| ID | Paper card | When to use |
|---:|---|---|
| 010 | [Spatial printing with continuous fiber (2024)](../../papers/cards/010-spatial-printing-continuous-fiber.md) | Continuous-fiber head on multi-axis / robot hardware; load paths matter more than cosmetics. |
| 015 | [Field-based toolpaths for CFRTPC (2021)](../../papers/cards/015-field-based-toolpaths-cfrtpc.md) | Continuous fiber–reinforced thermoplastic composite (CFRTPC) hardware; principal stress should drive fiber density and direction. |
| 022 | [Learning-based toolpath planner on graphs (2024)](../../papers/cards/022-learning-based-toolpath-planner-graphs.md) | Fiber or anisotropic bead graphs where combinatorial next-node choice (coverage, continuity, cut cost) is hard to hand-tune. |
| 027 | [Multi-layer carbon fiber pattern optimization (2024)](../../papers/cards/027-multi-layer-carbon-fiber-pattern-optimization.md) | Multi-layer continuous carbon-fiber parts where loop patterns must be packed without illegal overlaps. |
| 031 | [Non-planar CFRC review (2025)](../../papers/cards/031-non-planar-cfrc-review.md) | Orientation / literature card: survey non-planar continuous fiber–reinforced composites (CFRC) before picking #10/#15/#52/#27. |
| 052 | [High-density spatial fiber toolpaths (2024/25)](../../papers/cards/052-high-density-spatial-fiber-toolpaths.md) | Need dense, evenly spaced continuous fibers in 3D / on curved layers (not just adaptive sparse stress isocurves). |

## F-planar — Adaptive slicing / mesh formats

| ID | Paper card | When to use |
|---:|---|---|
| 002 | [Adaptive slicing via contour reconstruction (2021)](../../papers/cards/002-adaptive-slicing-contour-reconstruction.md) | Planar FFF job where fixed layer height leaves staircase or overfill on slopes, but the user stays on stock 3-axis hardware. |
| 003 | [Adaptive slicing for FDM revisited (Hamburg 2017)](../../papers/cards/003-adaptive-slicing-fdm-revisited.md) | User wants interactive control of adaptive planar heights (not only automatic cusp heuristics). |
| 023 | [Memory-efficient adaptive lattices (2021)](../../papers/cards/023-memory-efficient-adaptive-lattices.md) | Large lattice / TPMS-style parts that do not fit as a full dense mesh in slicer RAM. |
| 035 | [Optimal triangle mesh slicing](../../papers/cards/035-optimal-triangle-mesh-slicing.md) | Core planar slicer engine needs fast, robust contour extraction from triangle meshes. |
| 057 | [Survey of AM data representations (STL/AMF/3MF/CLI/STEP)](../../papers/cards/057-survey-am-data-representations.md) | Choosing import/export formats for the adaptive slicer (mesh vs AMF vs 3MF vs CLI vs STEP). |
| 058 | [Half-edge topology on STL soup for defect queries (2003)](../../papers/cards/058-half-edge-topology-stl-soup.md) | Ingested STL is a triangle soup; slicer must detect holes, non-manifold edges, inverted faces before adaptive slice. |

## F-toolpath — General toolpath planning

| ID | Paper card | When to use |
|---:|---|---|
| 009 | [Continuous toolpaths for sparse infill (2020)](../../papers/cards/009-continuous-toolpaths-sparse-infill.md) | Sparse lattice/infill where travel moves and crossovers hurt surface or strength. |
| 017 | [FullControl G-code Designer (2021)](../../papers/cards/017-fullcontrol-gcode-designer.md) | Research or power-user workflows that design extrusion geometry directly as G-code primitives. |
| 019 | [Image2Gcode (2025)](../../papers/cards/019-image2gcode.md) | Generate draft toolpath keypoints from images (sketches, photos of targets) for expert editing. |
| 021 | [Implicit toolpaths for functionally graded AM (2025)](../../papers/cards/021-implicit-toolpaths-functionally-graded-am.md) | Parts defined as OpenVCAD (or similar) geometry *and* material fields, not a single STL solid. |
| 034 | [Optimal toolpaths with thermal constraints (2020)](../../papers/cards/034-optimal-toolpaths-thermal-constraints.md) | Segment/region ordering must respect temperature bounds (avoid reheating too soon or printing on too-cold beads). |
| 040 | [Tension in spiderweb-inspired networks (2025)](../../papers/cards/040-tension-spiderweb-inspired-networks.md) | Designing printable TPU (or similar) networks that should carry tension only after assembly/stretch. |
| 053 | [Topology-preserving scalar field for spiral toolpaths (2025)](../../papers/cards/053-topology-preserving-scalar-field-spiral-toolpaths.md) | Need a single boundary-conforming spiral fill without singularities inside the region. |
| 055 | [Trajectory optimization for microstructure control (2024)](../../papers/cards/055-trajectory-optimization-microstructure-control.md) | Energy-beam processes (E-beam context in corpus) where power-field trajectories steer microstructure. |

## G — Topology optimization / DfAM

| ID | Paper card | When to use |
|---:|---|---|
| 047 | [Self-support TO considering distortion (2022)](../../papers/cards/047-self-support-to-considering-distortion.md) | Design-stage DfAM: optimize topology so the part is closer to self-supporting *and* less prone to process distortion before spending multi-axis slice budget. |
| 048 | [Self-supporting topology optimization (2017)](../../papers/cards/048-self-supporting-topology-optimization.md) | Early DfAM: force the topology to respect a maximum overhang angle so planar (or chosen-direction) printing needs fewer supports. |
| 050 | [Support-free hollowing via Voronoi of ellipses (2017)](../../papers/cards/050-support-free-hollowing-voronoi-ellipses.md) | Hollow a solid part while keeping internal voids self-supporting (no internal support structures). |

## VPP — Vat / volumetric / multi-axis DLP

| ID | Paper card | When to use |
|---:|---|---|
| 008 | [Computed Axial Lithography (2017)](../../papers/cards/008-computed-axial-lithography.md) | Volumetric vat photopolymerization (CAL) instead of layer-by-layer VPP. |
| 011 | [Curve-based slicer for multi-axis DLP (2025, SIGGRAPH Asia Best Paper)](../../papers/cards/011-curve-based-slicer-multi-axis-dlp.md) | Multi-axis DLP where layers are not global Z planes but local tangent planes along a space curve. |
| 014 | [Delta DLP with large size (2016)](../../papers/cards/014-delta-dlp-large-size.md) | Large DLP builds where a single projector FOV cannot cover the slice. |
| 025 | [Multi-axis AM for automotive components (2026)](../../papers/cards/025-multi-axis-am-automotive-components.md) | Automotive resin/DLP components needing curved iso-layers plus depth control. |
| 036 | [Overprinting with tomographic VAM (2025)](../../papers/cards/036-overprinting-tomographic-vam.md) | Volumetric additive manufacturing must cure around existing inserts / preforms. |
| 044 | [Roll-to-roll tomographic VAM (2024)](../../papers/cards/044-roll-to-roll-tomographic-vam.md) | Continuous-web volumetric production instead of batch vat CAL. |

## Process — Modeling / inspection / concrete

| ID | Paper card | When to use |
|---:|---|---|
| 024 | [Meshing framework for digital twins of extrusion AM (2025)](../../papers/cards/024-meshing-framework-digital-twins-extrusion-am.md) | Need an as-printed hex mesh from G-code for FEA / digital twin, not the ideal CAD mesh. |
| 059 | [ShapeGen3DCP (2025)](../../papers/cards/059-shapegen3dcp.md) | 3D concrete printing (3DCP) where bead shape depends on rheology and process parameters. |
| 060 | [Geometry/surface inspection in 3D concrete printing (review)](../../papers/cards/060-geometry-surface-inspection-3d-concrete-printing.md) | Designing QC loops for 3DCP cells (sensors, metrics, feedback). |
| 061 | [Digital chain in concrete 3D printing (2024)](../../papers/cards/061-digital-chain-concrete-3d-printing.md) | Standing up an end-to-end 3DCP workflow from design through helical slicing to FEM. |
| 062 | [Surface roughness prediction and visualization (2026)](../../papers/cards/062-surface-roughness-prediction-visualization.md) | Predict and visualize surface roughness per facet before printing (planning / DfAM feedback). |

## Chaining (quick)

- **F → A:** adaptive planar thickness / formats, then ZAA or Ahlers skins.
- **G → B / E:** self-supporting or orientation-aware geometry into curved layers or fiber fields.
- **B → E:** curved / stress layers → continuous-fiber packing (#10/#15/#52/#27).
- **E / B / C → D:** spatial fiber or multi-axis TCP → singularity-aware IK.
- **F toolpath (#9/#53/#21):** continuous / spiral / graded fill inside A/B/C layers.
- **VPP:** parallel vat/volumetric lane (CAL #8, multi-axis DLP #11/#25, overprint #36, R2R #44) — not FFF toolpath chain.
- **Process:** digital twin / QC / concrete (#24/#59–#62) after extrusion or 3DCP toolpaths.

## Inventory notes

Empty or missing registry links on cards:
- #31 Non-planar CFRC review (2025)
- #3 Adaptive slicing for FDM revisited (Hamburg 2017)
- #35 Optimal triangle mesh slicing
- #57 Survey of AM data representations (STL/AMF/3MF/CLI/STEP)
- #58 Half-edge topology on STL soup for defect queries (2003)
- #17 FullControl G-code Designer (2021)
- #14 Delta DLP with large size (2016)
- #52 DOI year listed 2024 in inventory but journal is 2025 — see card Notes.
- #57/#58: ScienceDirect S-numbers in card Notes (no stable DOI in registry).
- #31 is a review; prefer primary E methods for implementation.
