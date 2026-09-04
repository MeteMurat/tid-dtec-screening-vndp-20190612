# Reliability-Audited Screening of TID-Like Structures in GPS-Derived dTEC Maps

This repository accompanies the continuing development of the manuscript:

**Reliability-Audited Screening of TID-Like Structures in Dense GPS-Derived dTEC Maps: Sampling Density, Propagation, and Cross-Instrument Tests**

## Current manuscript scope

The revised study uses a fixed master network of 435 dual-frequency GPS stations over 10–14 June 2019 (DOY 161–165), with carrier-phase dTEC as the primary measurement branch and code-derived dTEC as a comparison branch. The reliability audit includes interpolation sensitivity, screening-parameter sensitivity, five-day transportability, baseline-method comparisons, physical-propagation estimator comparison, an IPP sampling-geometry null, geomagnetic/solar context, an independent PA836 ionosonde comparison, and controlled receiver-density degradation.

The manuscript treats “moderate” and “strong” only as predefined numerical screening-support states. They are not independently confirmed TID labels, and no human- or AI-generated labels are used as physical ground truth.

## Public release v1.1.0

The existing public release **v1.1.0** is retained as a legacy reproducibility/supplementary archive for the earlier single-day exploratory stage of the project (12 June 2019). It contains the archive `tid_dtec_screening_reproducibility_v1.1.0.zip` together with the earlier supplementary videos and still images.

Because the current manuscript substantially expands the analysis to a five-day, dense-network reliability audit, **v1.1.0 should not be treated as the complete reproducibility package for the current manuscript**. A new versioned release containing the revised five-day analysis products should be deposited in this repository before final publication/submission of the reproducibility package.

## Data provenance

Raw GPS RINEX and broadcast-navigation data are obtained from the NOAA National Geodetic Survey CORS Network public archive. The independent PA836 ionosonde comparison uses the official NOAA/NCEI archive. Geomagnetic and solar indices are used only as contextual data and are not used to retune candidate windows or screening thresholds.

## Legacy release

- v1.1.0: https://github.com/MeteMurat/tid-dtec-screening-vndp-20190612/releases/tag/v1.1.0

