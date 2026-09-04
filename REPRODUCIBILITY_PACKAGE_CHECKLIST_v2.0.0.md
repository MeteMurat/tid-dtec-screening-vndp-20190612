# Reproducibility Package Checklist — v2.0.0

This checklist defines the minimum public archive expected for the revised five-day dense-network manuscript. Items should be frozen before the GitHub release is published.

## Core reproducibility material

- [ ] Exact analysis source code used for the manuscript.
- [ ] Python/package environment specification with version numbers.
- [ ] 435-station master receiver list.
- [ ] Daily station-availability records for 10–14 June 2019.
- [ ] Source-data inventory and provider metadata for GPS RINEX/navigation inputs.
- [ ] Fixed grid/interpolation configuration.
- [ ] Complete 71-window candidate table with immutable date/start/end/duration fields.

## Reliability-audit products

- [ ] Dense-network spatial-support diagnostics.
- [ ] Interpolation-sensitivity scenario table and per-scenario outputs.
- [ ] Screening coefficient/threshold sensitivity and ablation outputs.
- [ ] Carrier-phase/code comparison tables and frozen map products.
- [ ] Five-day transportability tables.
- [ ] Simpler baseline-comparison tables.
- [ ] Physical-propagation estimator outputs.
- [ ] IPP-motion and stationary-field sampling-geometry-null outputs.
- [ ] Geomagnetic/solar contextual time series and source metadata.
- [ ] PA836 ionosonde input inventory, derived standardized residuals, and window-level comparison table.
- [ ] Controlled receiver-density degradation outputs for 100%, 75%, 50%, 25%, and 10% retention.

## Publication products

- [ ] Final manuscript figures in publication format.
- [ ] Figure-generation scripts/resources.
- [ ] Final manuscript tables in machine-readable CSV/JSON form where applicable.
- [ ] Provenance records linking figures/tables to the exact frozen products used.
- [ ] Claim-boundary/read-me document describing what the release does and does not validate.

## Integrity and release freeze

- [ ] Single final reproducibility archive created after all above items are frozen.
- [ ] SHA-256 digest generated for the archive.
- [ ] Machine-readable SHA-256 manifest generated for individual distributed products.
- [ ] Archive extracted into a clean directory and smoke-tested.
- [ ] No stale single-day exploratory labels are presented as current validation truth.
- [ ] No human- or AI-generated labels are presented as independent ground truth.
- [ ] README and release notes match the final manuscript title and scope.
- [ ] Manuscript Data and code availability statement matches the exact published release tag and archive name.

## Planned release

Target release tag: `v2.0.0`

Legacy release `v1.1.0` remains available for the earlier single-day exploratory stage and should not be used as the complete reproducibility package for the revised five-day manuscript.
