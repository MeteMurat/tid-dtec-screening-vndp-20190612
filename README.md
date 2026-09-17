# Reliability Auditing and Temporal Transportability of GPS-Derived Ionospheric Disturbance Mapping

This repository accompanies the manuscript:

**Reliability Auditing and Temporal Transportability of GPS-Derived Ionospheric Disturbance Mapping: Sampling, Propagation, and Cross-Instrument Constraints**

## Current manuscript scope

The study is organized as two deliberately distinct evidence tiers.

### 1. Five-day dense map-level reliability audit

The map-level analysis uses a fixed master network of 435 dual-frequency GPS stations over 10--14 June 2019 (DOY 161--165), with carrier-phase dTEC as the primary measurement branch and code-derived dTEC as a common-geometry comparison branch. The fixed five-day campaign contains 71 predefined TID-like candidate windows on a 28 x 40 grid at 5 min cadence.

The reliability audit includes:

- dense-network spatial-support diagnostics;
- controlled interpolation sensitivity;
- carrier-phase/code measurement-branch consistency;
- screening-rule sensitivity;
- dense-campaign rule transport across all five dates;
- amplitude, projected-keogram, and spectral-peak comparator baselines;
- independent physical-propagation estimator comparison;
- a stationary-field IPP sampling-geometry null;
- geomagnetic/solar contextualization;
- independent PA836 ionosonde comparison; and
- controlled receiver-density degradation.

The terms **moderate** and **strong** denote predefined numerical screening-support states only. They are not independently confirmed TID classes. The 435-station reconstruction is treated as the highest-support reproducibility reference, not as physical ground truth.

### 2. Multi-year pointwise temporal-transportability extension

A separately prespecified pointwise-processing experiment evaluates 48 dates spanning 2018--2024 using three fixed, outcome-blind validation receivers per date (144 receiver-days). All 48 dates produced non-empty pointwise dTEC products.

This extension tests **operational pointwise-processing transportability only**. It is not a 48-date full-network remapping experiment and is not used to infer regional map reproducibility, TID occurrence rates, climatology, or independently confirmed physical event identity.

The 48-date extension post-dates the frozen `v2.0.0` five-day reproducibility release and is therefore not represented by the standalone assets of that release.

## Public reproducibility release v2.0.0

Release **v2.0.0** is the frozen reproducibility package for the five-day dense-network reliability audit and is publicly available here:

- https://github.com/MeteMurat/tid-dtec-screening-vndp-20190612/releases/tag/v2.0.0

Canonical archive:

`tid_dtec_screening_reproducibility_v2.0.0_20260904_105618.zip`

Verified SHA-256:

`6103BD696697CA6E22AFFB8751FAC87116938ED30DC65D1B0D2883BBB8734085`

A companion `.sha256` file is distributed with the release.

The release contains the fixed 435-station master list and daily availability records, candidate-window tables, versioned analysis code, software-environment information, interpolation- and screening-sensitivity products, carrier-phase/code comparison products, physical-propagation diagnostics, the stationary-field IPP sampling-geometry null analysis, five-day comparator and contextual analyses, receiver-density degradation results, publication-figure resources, and machine-readable provenance records.

Scientific scope and interpretation boundaries are documented in [`RELEASE_NOTES_v2.0.0.md`](RELEASE_NOTES_v2.0.0.md), with package-completeness information in [`REPRODUCIBILITY_PACKAGE_CHECKLIST_v2.0.0.md`](REPRODUCIBILITY_PACKAGE_CHECKLIST_v2.0.0.md).

## Legacy supplementary-video release v1.1.0

Release **v1.1.0** is retained unchanged as a legacy archive for the earlier single-day exploratory stage (12 June 2019). It should **not** be treated as the complete reproducibility package for the current manuscript.

- https://github.com/MeteMurat/tid-dtec-screening-vndp-20190612/releases/tag/v1.1.0

The following supplementary animations remain publicly preserved in that release:

- `Video_S1_Event14.mp4` -- event-focused supplementary animation
- `Video_S2_ModerateCandidates.mp4` -- earlier moderate-candidate visualization
- `Video_S3_ArtifactAblation.mp4` -- earlier artifact-ablation visualization

Paired still images are also distributed for all three videos.

Direct Event 14 movie asset:

- https://github.com/MeteMurat/tid-dtec-screening-vndp-20190612/releases/download/v1.1.0/Video_S1_Event14.mp4

These legacy animations are retained as supplementary visualizations only. They are not quantitative validation targets, independent physical evidence, or inputs to the five-day dense-network or 48-date temporal-transportability analyses reported in the current manuscript.

## Data provenance

Raw GPS RINEX observations and broadcast-navigation data for the five-day dense campaign are obtained from the NOAA National Geodetic Survey CORS Network public archive. The independent PA836 ionosonde comparison uses the official NOAA/NCEI archive. Geomagnetic and solar indices are used only as contextual data and are not used to retune candidate windows, interpolation settings, or screening thresholds.

## Interpretation boundary

This repository is intended to preserve reproducibility and provenance, including unfavorable or internally inconsistent results. It does not convert screening-support states into independently confirmed physical TID labels. Carrier-phase/code agreement, propagation-estimator disagreement, sampling-geometry diagnostics, ionosonde non-concordance, and temporal processing success are retained as distinct forms of evidence rather than collapsed into a single validation claim.
