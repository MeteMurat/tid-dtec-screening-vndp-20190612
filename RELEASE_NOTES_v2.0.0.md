# v2.0.0 — Five-Day Dense-Network Reliability Audit

**Status:** release-candidate documentation for the revised manuscript. The binary/source package should be uploaded as a new GitHub release asset only after the final reproducibility archive is frozen and its SHA-256 manifest is generated.

## Manuscript scope

This release corresponds to the revised manuscript:

**Reliability-Audited Screening of TID-Like Structures in Dense GPS-Derived dTEC Maps: Sampling Density, Propagation, and Cross-Instrument Tests**

The revised analysis uses a fixed master network of 435 dual-frequency GPS stations over 10–14 June 2019 (DOY 161–165). Carrier-phase dTEC is the primary measurement branch and code-derived dTEC is retained as a measurement-consistency comparison.

## Scientific analyses represented in v2.0.0

- Five-day dense-network GPS dTEC reconstruction on a fixed 28 × 40 grid at 5 min cadence.
- Complete predefined candidate universe of 71 windows without downstream candidate replacement or retiming.
- Spatial-support and nearest-IPP diagnostics.
- Thirteen-scenario interpolation sensitivity audit.
- Sixty-five-scenario screening coefficient/threshold sensitivity and component-ablation audit.
- Carrier-phase versus code-derived dTEC consistency analysis.
- Five-day transportability analysis.
- Simpler amplitude, projected-keogram, and spectral-peak baseline comparisons.
- Independent physical-propagation estimator comparison for the predefined 12 June 2019 midday case-study window.
- IPP-motion and stationary-field sampling-geometry null analysis.
- Geomagnetic/solar context using Kp, Dst, SYM-H, and observed F10.7.
- Independent PA836 ionosonde comparison using foF2 and hmF2 variability.
- Controlled receiver-density degradation at 100%, 75%, 50%, 25%, and 10% station retention.
- Publication figure-generation resources and provenance records.

## Principal interpretation boundaries

The release is designed to preserve unfavorable and inconclusive outcomes rather than optimize them away.

- “Moderate” and “strong” are predefined numerical screening-support states, not independently confirmed TID labels.
- The 435-station reconstruction is the highest-support reproducibility reference, not physical ground truth.
- Carrier-phase and code-derived dTEC are not treated as interchangeable map products.
- The code-derived branch is not an independent validation instrument because it shares the same GPS observing geometry.
- The two physical-propagation estimators are not averaged or post hoc selected when they disagree.
- The IPP/sampling-geometry null is a confounding analysis and does not establish an authoritative physical propagation vector.
- The independent PA836 ionosonde comparison does not establish positive aggregate concordance and is retained as negative external evidence.
- No independent blinded human relabeling study is used as validation ground truth.
- Classification-accuracy metrics such as sensitivity, specificity, precision, recall, F1 score, and ROC-AUC are not reported because no independent binary truth set exists.

## Key quantitative outcomes represented in the manuscript

- 435-station master GPS network; 423–435 valid station products per day.
- 71 predefined candidate windows across 10–14 June 2019.
- 12 June median geometry-supported grid fraction: 100%; minimum: 96.88%.
- Carrier-phase/code pooled Pearson correlation: 0.615; frame-centered pooled correlation: 0.609.
- Receiver-density median spatiotemporal Pearson correlation relative to the full-network reference: 0.945 at 75%, 0.801 at 50%, 0.580 at 25%, and 0.334 at 10% retention.
- Corresponding nearest-IPP-distance inflation factors: approximately 1.15, 1.56, 2.49, and 4.12.
- Independent physical estimators produce incompatible propagation parameterizations for the predefined midday case study.
- Median native same-link IPP speed: 94.2 m s^-1; 95th percentile: 308.4 m s^-1.
- Independent PA836 ionosonde variability is finite for 42 of 71 candidate windows, with no positive aggregate concordance established.

## Expected release assets

The final v2.0.0 release should contain a single frozen reproducibility archive and a machine-readable SHA-256 manifest. The archive should include the exact analysis code and environment specification; the 435-station master list and daily availability records; predefined candidate-window tables; interpolation- and screening-sensitivity products; carrier-phase/code consistency products; physical-propagation and IPP-geometry-null outputs; five-day baseline, geomagnetic, ionosonde, and density-degradation results; publication figures and figure-generation resources; and provenance/adjudication records needed to reproduce the manuscript tables and figures.

## Relationship to v1.1.0

Release `v1.1.0` is retained unchanged as a legacy archive for the earlier single-day exploratory stage. It should not be cited as the complete reproducibility package for the revised five-day manuscript. The revised manuscript should cite the new v2.0.0 release after its final archive and SHA-256 manifest are uploaded.
