# Reproducibility Package Checklist — v2.0.0

**Status:** published and frozen.

This document records the intended completeness criteria for the five-day dense-network reproducibility package that was subsequently published as release `v2.0.0`. It is retained as provenance for the release-freeze process rather than as a current to-do list.

## Published release

- Release tag: `v2.0.0`
- Release page: https://github.com/MeteMurat/tid-dtec-screening-vndp-20190612/releases/tag/v2.0.0
- Canonical archive: `tid_dtec_screening_reproducibility_v2.0.0_20260904_105618.zip`
- Archive size: 361,108,480 bytes
- Verified SHA-256: `6103BD696697CA6E22AFFB8751FAC87116938ED30DC65D1B0D2883BBB8734085`
- Companion checksum file: `tid_dtec_screening_reproducibility_v2.0.0_20260904_105618.zip.sha256`
- Clean-extract verification: PASS

The scientific scope and interpretation boundaries of the frozen package are documented in [`RELEASE_NOTES_v2.0.0.md`](RELEASE_NOTES_v2.0.0.md).

## Core reproducibility criteria used for the release freeze

The package was designed to preserve:

- exact analysis source code and software-environment information;
- the fixed 435-station master receiver list;
- daily station-availability records for 10--14 June 2019;
- source-data inventory and provider metadata for GPS RINEX/navigation inputs;
- fixed grid/interpolation configuration;
- the complete 71-window candidate universe with frozen timing fields; and
- machine-readable integrity and provenance records.

## Reliability-audit criteria used for the release freeze

The frozen five-day package was designed to include the evidence needed to trace:

- dense-network spatial-support diagnostics;
- interpolation-sensitivity outputs;
- screening coefficient/threshold sensitivity and component-ablation outputs;
- carrier-phase/code comparison products;
- five-day dense-campaign rule-transport results;
- simpler baseline comparisons;
- physical-propagation estimator outputs;
- IPP-motion and stationary-field sampling-geometry-null outputs;
- geomagnetic/solar contextual information;
- PA836 ionosonde cross-check products; and
- controlled receiver-density degradation at 100%, 75%, 50%, 25%, and 10% retention.

## Publication and integrity criteria

The release-freeze process required publication-figure resources, machine-readable provenance, archive-level SHA-256 verification, clean extraction, and preservation of the manuscript's interpretation boundaries. In particular:

- the 435-station reconstruction is a high-support reproducibility reference, not physical ground truth;
- “moderate” and “strong” are numerical screening-support states, not independently confirmed TID labels;
- no human- or AI-generated label is treated as independent physical ground truth; and
- unfavorable, null, or internally inconsistent reliability outcomes are preserved rather than optimized away.

## Scope boundary relative to the current manuscript

Release `v2.0.0` is the frozen reproducibility package for the **five-day dense-network reliability audit**. The current manuscript additionally contains a later, separately prespecified **48-date pointwise temporal-transportability extension spanning 2018--2024**. That later extension is not represented by the standalone assets of `v2.0.0` and should not be inferred from this checklist.

## Relationship to v1.1.0

Release `v1.1.0` remains available as a legacy archive for the earlier single-day exploratory stage. It also preserves the earlier supplementary animations and paired still images. It should not be cited as the complete reproducibility package for the current manuscript.
