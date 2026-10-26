<p align="center">
  <img src="sarproc_logo.png" alt="SARPROC logo: a radar satellite above an egg-shaped Earth" width="200">
</p>

# SARPROC

[![Sentinel-1: C-band](https://img.shields.io/badge/Sentinel--1-C--band-0B4F9C?style=flat-square)](https://www.esa.int/Applications/Observing_the_Earth/Copernicus/Sentinel-1)
[![BIOMASS: P-band](https://img.shields.io/badge/BIOMASS-P--band-2E7D32?style=flat-square)](https://www.esa.int/Applications/Observing_the_Earth/FutureEO/Biomass)
[![TanDEM-X: X-band](https://img.shields.io/badge/TanDEM--X-X--band-6A1B9A?style=flat-square)](https://www.dlr.de/en/research-and-transfer/projects-and-missions/tandem-x)
[![NISAR: L and S-band](https://img.shields.io/badge/NISAR-L%20%2B%20S--band-C62828?style=flat-square)](https://nisar.jpl.nasa.gov)
<br>
[![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![ESA SNAP](https://img.shields.io/badge/ESA-SNAP-003247?style=flat-square)](https://step.esa.int/main/toolboxes/snap/)
[![ESA MAAP](https://img.shields.io/badge/ESA-MAAP-003247?style=flat-square)](https://portal.maap.eo.esa.int)
[![HPC: Slurm](https://img.shields.io/badge/HPC-Slurm-1F6FB2?style=flat-square)](https://slurm.schedmd.com)
[![made in Wageningen](https://img.shields.io/badge/made%20in-Wageningen-34B233?style=flat-square)](https://www.wur.nl)
[![WENR: Earth Informatics](https://img.shields.io/badge/WENR-Earth%20Informatics-E8B848?style=flat-square)](https://www.earthinformatics.eu)

Processing chains for synthetic aperture radar (SAR) satellite data: from raw or Level-1 products to
analysis-ready results for forest, vegetation and land monitoring.

SARPROC is run by the team **Earth Observation and Environmental Informatics** of
**Wageningen Environmental Research (WENR)**, part of **Wageningen University & Research (WUR)**.

## Missions

| Repository | Mission | Band | What it does |
|---|---|---|---|
| **Sentinel-1** | Copernicus Sentinel-1 | C | ESA SNAP processing of large areas and long time series on an HPC cluster |
| **BIOMASS** | ESA BIOMASS | P | finds products in the ESA MAAP catalogue, checks stack coverage, runs the BIOMASS Processing Suite from L0 to L2A forest products, and SAR tomography |
| **TanDEM-X** | DLR TanDEM-X | X | planned |
| **NISAR** | NASA-ISRO NISAR | L, S | planned |

## How we work

- **Python**, with reproducible environments and unit tests that run offline.
- **Heavy processing on the WUR HPC cluster** (Slurm); one self-continuing job chain per stack or
  tile, safe to restart after a failure.
- **Traceable products**: every result carries the IDs of its input products and the processor
  version used.
- **Documentation for users**, not only for developers: the steps should be clear to someone without
  HPC experience.

Some repositories are private while the work is ongoing.

## Contact

Team Earth Observation and Environmental Informatics, Wageningen Environmental Research:
[www.earthinformatics.eu](https://www.earthinformatics.eu)

Wageningen Environmental Research: [wur.nl/environmental-research](https://www.wur.nl/en/research-results/research-institutes/environmental-research.htm)
