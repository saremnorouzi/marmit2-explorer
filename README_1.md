# MARMIT-2 Wet Soil Reflectance Explorer

**Open the app:** https://saremnorouzi.github.io/marmit2-explorer/

An interactive, browser-based visualisation of the MARMIT-2 radiative transfer model (Dupiau et al., 2022), showing how a thin water layer changes the reflectance spectrum of a soil (400–2400 nm). Move the sliders, or drag the water layer, to vary the three model parameters:

- **L**: water-layer thickness (cm)
- **ε**: wet surface fraction
- **δ**: volume fraction of soil particles in the water layer

Nothing to install. The app runs in any modern browser. For offline use, click **Download for offline use** in the app, or download `index.html` from this repository, then double-click the file.

## Model and data

Reflectance is computed exactly as in the official MARMIT-2 Python function `get_spectrum`. The JavaScript implementation was verified against the reference code to machine precision (maximum absolute difference about 3 × 10⁻¹⁵) on four dry soils × 4,150 parameter sets, including all fitted parameter sets of the eight MARMIT-2 validation databases.

- Water refractive index: Segelstein (1981)
- Water absorption: Buiteveld et al. (1994), Kou et al. (1993), Wieliczka et al. (1989)
- Dry soil spectra: Bablet et al. (2018) database

**Reference:** Dupiau A., Jacquemoud S., Briottet X., Fabre S., Viallefont-Robinet F., Philpot W., Di Biagio C., Hébert H., Formenti P. (2022). MARMIT-2: an improved version of the MARMIT model to predict soil reflectance as a function of surface water content in the solar domain. *Remote Sensing of Environment*, 272, 112951. https://doi.org/10.1016/j.rse.2022.112951

## Contact

Web implementation by Sarem Norouzi (Aarhus University): sarem.nrz@gmail.com
