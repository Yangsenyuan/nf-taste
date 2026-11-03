# Corpus Evidence

This file documents where the rules come from, so any rule can be checked rather
than trusted.

## Paper index

| ID | Year | Journal | Title |
|---|---|---|---|
| P01 | 2015 | Remote Sensing of Environment | Applicability of the PROSPECT model for estimating protein and cellulose + lignin in fresh leaves |
| P02 | 2017 | Remote Sensing of Environment | Examining spectral reflectance features related to Arctic percent vegetation cover |
| P03 | 2019 | Remote Sensing of Environment | Mapping foliar functional traits and their uncertainties across three years |
| P04 | 2021 | Remote Sensing of Environment | Hyperspectral imagery to monitor crop nutrient status within and across seasons |
| P05 | 2023 | Remote Sensing of Environment | Generality of leaf spectroscopic models for predicting key foliar functional traits |
| P06 | 2026 | Remote Sensing of Environment | Enhancing transferability of foliar trait retrieval models |
| P07 | 2025 | Computers and Electronics in Agriculture | Characterizing key foliar functional traits of subtropical evergreen forests |
| P08 | 2016 | International Journal of Applied Earth Observation and Geoinformation | Modelling high arctic percent vegetation cover using field digital images |
| P09 | 2016 | International Journal of Applied Earth Observation and Geoinformation | Canopy foliar nitrogen retrieved from airborne hyperspectral imagery |
| P10 | 2018 | International Journal of Applied Earth Observation and Geoinformation | Remote sensing of Arctic percent vegetation cover and fAPAR on Baffin Island |
| P11 | 2021 | International Journal of Applied Earth Observation and Geoinformation | Trail camera networks provide insights into satellite-derived phenology |
| P12 | 2023 | ISPRS Journal of Photogrammetry and Remote Sensing | Multi-year hyperspectral remote sensing of crop functional traits |
| P13 | 2024 | International Journal of Applied Earth Observation and Geoinformation | Multi-source satellite remote sensing for monitoring foliar traits |
| P14 | 2025 | International Journal of Applied Earth Observation and Geoinformation | Transfer learning for enhancing the generality of leaf spectroscopic models |
| P15 | 2024 | Forest Ecosystems | Quantifying foliar trait variation and covariation in sun and shade leaves |
| P16 | 2013 | Hydrology and Earth System Sciences | A statistics-based temporal filter algorithm for spatiotemporally continuous mapping |
| P17 | 2015 | IEEE JSTARS | Leaf nitrogen content indirectly estimated by leaf traits derived from PROSPECT |
| P18 | 2018 | Agricultural and Forest Meteorology | Mapping forest canopy nitrogen content by inversion of coupled leaf-canopy models |
| P19 | 2026 | ISPRS Journal of Photogrammetry and Remote Sensing | Advancing hyperspectral nutrient modeling through transfer learning |
| P20 | 2020 | New Phytologist | Foliar functional traits from imaging spectroscopy across biomes |
| P21 | 2025 | Remote Sensing | Assessing the transferability of models for predicting foliar nutrient concentrations |
| P22 | 2025 | Remote Sensing | Mechanisms of hyperspectral remote sensing for belowground traits |
| P23 | 2026 | Remote Sensing | Evaluating airborne and UAV-based imaging spectroscopy for grassland traits |
| P24 | 2026 | Remote Sensing | Scaling foliar phenolics from airborne imaging spectroscopy to Sentinel-2 |

## Evidence format

`P07-DIS-P003` = paper 07, Discussion section, paragraph 3.

Section tags used in IDs:

| Tag | Section |
|---|---|
| ABS | Abstract |
| INT | Introduction |
| MET | Materials and Methods |
| RES | Results |
| DIS | Discussion |
| CON | Conclusion |
| CAP | Figure/table caption |

## How the counts were produced

- 24 PDFs, parsed to section-tagged paragraphs; references, tables, captions,
  back matter, and running headers excluded from prose statistics.
- 1,609 prose paragraphs; 7,205 sentences.
- Counts are `paragraphs / papers`. A pattern is only promoted to `Confirmed`
  when it appears in at least 8 papers and has no large body of counter-examples.
- Percentages are always given with their denominator. A bare percentage is not
  evidence.

## What the corpus cannot support

- **No claim about author identity.** Rules describe the group's published
  writing, not an individual's style.
- **No claim about unpublished preferences.** If a pattern is absent from the 24
  papers, the rule files say `general convention`, not "the group does this".
- **No claim about section structure that the corpus contradicts.** 3/24 papers
  combine Results and Discussion; the rules allow that.

## Known extraction limitations

- Two papers (P08, P09) have a word-per-block text layer; reading order was
  rebuilt from coordinates, and paragraph boundaries there may be coarser than
  in the others.
- Captions are indexed but not all are attached to a figure number.
- Author lists and affiliations are not indexed.
