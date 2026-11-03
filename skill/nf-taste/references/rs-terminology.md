# Vegetation Remote Sensing Terminology

Scope: terms this corpus actually uses, their collocations, and the
near-synonyms that must not be treated as interchangeable.

Counts are occurrences / papers. Terms marked `general convention` are standard
domain usage, not corpus-specific findings.

---

## Traits and vegetation quantities

| Term | Corpus usage | Note |
|---|---|---|
| foliar functional traits | 982 occurrences / 18 papers (`foliar`) | Umbrella term for leaf-level traits; keep as the framing term in Introduction |
| leaf traits | common | Use when the measurement is at leaf level; do not rotate with "foliar traits" |
| canopy traits | common | Use only when the measurement integrates the canopy |
| LAI (leaf area index) | m² m⁻² | Structural; not a proxy for biomass |
| FVC / PVC / vegetation cover | percent cover | The corpus uses both "fractional vegetation cover" and "percent vegetation cover"; pick one and define it |
| biomass / aboveground biomass | g m⁻² or kg m⁻² | Always state dry/wet and per-area basis |
| foliar nitrogen (N) | 645 occurrences / 19 papers (`nitrogen`) | Specify mass-based (%, mg g⁻¹) vs area-based (g m⁻²); they are not interchangeable |
| chlorophyll | 277 / 21 | Specify a/b total vs chlorophyll content per area |
| dry matter (LMA) | 117 / 19 | LMA is leaf mass per area; dry matter content is a fraction — different quantities |
| water content (EWT) | common | Equivalent water thickness (cm) vs gravimetric water content (%) — do not mix |
| pigments / carotenoids | common | Report which pigment and which retrieval basis |

## Spectral quantities

| Term | Usage | Note |
|---|---|---|
| reflectance | 653 occurrences / 24 papers (`spectral`) | Directional–hemispherical reflectance (DHR) vs bidirectional reflectance factor (BRF) are different; the corpus distinguishes them explicitly |
| transmittance | common | Leaf-level; state whether directional or hemispherical |
| BRF | common | Do not shorten to "reflectance" when the geometry matters |
| absorption coefficient | common | Specific absorption coefficient is per unit content; state the unit |
| spectral resolution / sampling interval | common | nm; distinguish FWHM from band spacing |
| VNIR / SWIR | common | State the wavelength ranges used |

## Indices and products

| Term | Usage | Note |
|---|---|---|
| NDVI, EVI, SAVI | common | Write the acronym out at first use; do not use "vegetation index" and "VI" interchangeably in the same paragraph |
| GPP / NPP | common | GPP is gross uptake; NPP is net production after respiration — not synonyms |
| fAPAR | common | Fraction of absorbed photosynthetically active radiation; do not conflate with FVC |
| SOS / EOS / LOS | common | Phenology transition dates; define the threshold method |

## Sensors and platforms

| Term | Usage | Note |
|---|---|---|
| hyperspectral | 189 occurrences / 19 papers | Prefer to "imaging spectroscopy" only when the paper uses that term consistently |
| multispectral | common | State the number of bands |
| airborne / UAV-borne / spaceborne | common | "UAV" and "drone" — use UAV |
| Sentinel-2 MSI, Landsat OLI, MODIS | common | Name the product and level (L1C, L2A, surface reflectance) |

## Modelling and validation

| Term | Usage | Note |
|---|---|---|
| calibration | 140 occurrences / 20 papers | Fitting the model |
| validation | 173 / 21 | Independent evaluation; do not use "validation" for cross-validation on the same data without saying so |
| cross-validation | common | State k and the partitioning scheme |
| estimation / retrieval / prediction | 215 / 22 (`estimation`) | Estimation and retrieval are often interchangeable in this corpus; prediction implies a new sample. Keep one term per paper |
| inversion | common | Model inversion (radiative transfer) is not statistical fitting |
| RMSE / NRMSE / MAE / R² | 166 / 20 (`rmse`), 382 / 22 (`r2`) | Always give units and the sample the metric was computed on |
| uncertainty | common | Distinguish measurement uncertainty from model uncertainty |
| transferability | common | The ability of a model trained in one setting to perform in another; define the transfer scenario |

## Near-synonyms that must stay distinct

- **estimation vs retrieval vs prediction** — pick one per paper; do not rotate.
- **reflectance vs BRF** — geometry-dependent; not interchangeable.
- **LAI vs FVC vs biomass** — structure, cover, and mass are different quantities.
- **GPP vs NPP** — different carbon fluxes.
- **validation vs calibration** — different datasets and purposes.
- **accuracy vs precision** — accuracy is closeness to truth; precision is
  repeatability.

## Collocations observed in the corpus

- `retrieve X from Y` (not "retrieve X by Y")
- `estimate X using Y` / `estimate X from Y`
- `map X across Y`
- `model performance` / `model accuracy`
- `spectral feature` / `spectral region` / `spectral subset`
- `independent validation` / `independent dataset`
- `cross-species transferability` / `model transferability`
- `ill-posed inverse problem`
- `radiative transfer model inversion`
