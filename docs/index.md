# IND — VerveStacks Model

!!! info "Model Info"
    **Generated:** 2026-06-03 22:34:54  |  **ISO Code:** `IND`

---

## Model Calibration 2022

| **Total Capacity** | **Total Generation** | **CO2 Emissions** | **Calibration to EMBER** |
|--------------|---------------|------------|--------------------------|
| 441 GW | 1829 TWh | 1296 Mt | 101% |

> **Note:** 2022 fossil and bio capacity is calibrated to EMBER and renewable capacities to IRENA.
> UNSD has incomplete data for fuel consumption, so calibration is demonstrated against total CO₂ emissions
> reported by EMBER — confirming that efficiency assumptions are sound.

---

## Power Generation Assets

### Existing Capacity

| **Fuel Type** | **Threshold** | **Plants Above Threshold** | **Active Capacity** | **Mothballed Capacity** | **Wtd Avg Efficiency** |
|---------------|---------------|----------------------------|--------------------|--------------------------|-----------------|
| 🌱 **Bioenergy** | 50 MW | 20/30 plants | 10.7 GW | — | 34.2% |
| ⚫ **Coal** | 500 MW | 316/728 plants | 273 GW | 0.582 GW | 37.1% |
| 🔥 **Gas** | 500 MW | 18/106 plants | 32.6 GW | — | 48.7% |
| 💧 **Hydro Power** | 110 MW | 137/235 plants | 58 GW | 2.97 GW | 94% |
| ⚛️ **Nuclear** | — | 31/31 plants | 13.4 GW | 0.64 GW | 100% |
| 🛢️ **Oil** | 500 MW | 0/6 plants | 0.656 GW | — | 38.8% |
| ☀️ **Solar** | 200 MW | 248/721 plants | 107 GW | — | 99% |
| 💨 **Windon** | 200 MW | 89/226 plants | 52 GW | — | 89% |
| 🔋 **Pumped Storage** | 110 MW | 12/13 plants | 8.13 GW | — | 100% |


### Future Projects (offered for endogenous selection)

| **Fuel Type** | **Threshold** | **Plants Above Threshold** | **Total Capacity** | **Wtd Avg Efficiency** |
|---------------|---------------|----------------------------|--------------------|-----------------|
| 🌱 **Bioenergy** | 50 MW | 2/3 plants | 0.14 GW | 30.7% |
| ⚫ **Coal** | 500 MW | 104/108 plants | 81 GW | 40.5% |
| 🔥 **Gas** | 500 MW | 1/2 plants | 0.9 GW | 57% |
| 💧 **Hydro Power** | 110 MW | 111/134 plants | 75 GW | 100% |
| ⚛️ **Nuclear** | — | 24/24 plants | 25.8 GW | 100% |
| ☀️ **Solar** | 200 MW | 103/155 plants | 73 GW | 100% |
| 🌊 **Windoff** | 200 MW | 6/6 plants | 5 GW | 100% |
| 💨 **Windon** | 200 MW | 20/33 plants | 8.34 GW | 100% |
| 🔋 **Pumped Storage** | 110 MW | 52/52 plants | 61 GW | 100% |


Announced and pre-construction projects are offered as options to the model for endogenous investment.
This is particularly useful for hydro and pumped storage where country-wise potential is not readily
available. Grid locations of all these units are preserved.

### CCS Retrofit Potential

| Fuel | Retrofit Host Capacity | Retrofit Potential |
|------|------------------------|-------------------|
| ⚫ **Coal** | 274 GW | 192 GW after capacity penalty |
| 🔥 **Gas**  | 32.6 GW  | 27.6 GW after capacity penalty |

---

## Data Sources & Coverage

### Base-Year Power Plant Specifications

- **Global Energy Monitor (GEM)** — Open-access database of individual power plants worldwide,
  including location, capacity, fuel type, commissioning year, and technical specifications.
- **International Renewable Energy Agency (IRENA)** — Global renewable energy capacity and generation
  statistics (2000–2022), disaggregated by country and technology.
- **EMBER Climate** — Global dataset tracking electricity generation, installed capacity, and emissions
  intensity (2000–2022).

### Enhanced Renewable Energy Characterization

- **GEM–REZoning–Atlite Integration** — Renewable energy units enriched with capacity factors from
  Atlite weather data and precise grid-cell locations from the REZoning database.
- Individual renewable plants receive location-specific capacity factors derived from 2013 hourly
  weather patterns.
- Plants mapped to 50×50 km REZoning grid cells for consistent spatial modelling.

### Data Processing Notes

| Metric | Value |
|--------|-------|
| **Individual Plant Coverage** | 97% of total capacity from plant-level GEM data |
| **Total Capacity Tracked** | 891 GW from all sources |
| **Plants Above Threshold** | 1836 individual plants tracked |
| **Total Plants Processed** | 2613 plants in database |
| **Missing Capacity Added** | - **IRENA data**:
  - **hydro**: 3.43 GW
  - **bioenergy**: 9.99 GW
  - **windon**: 8.92 GW
  - **solar**: 1.1 GW
- **EMBER data**:
  - **gas**: 1.39 GW |

---

## Model Files

- **Source Data:** `source_data/VerveStacks_IND.xlsx` — full dataset in a model-agnostic format
- **VEDA Model Files:** Complete model ready for Veda-TIMES execution
- **Scenario Files:** AR6 climate scenarios and policy assumptions

---

## Quality Assurance

- Cross-validation between IRENA, EMBER, and UNSD statistics
- Capacity-generation consistency checks
- Technology classification verification
- Historical data reconciliation for base year (2022)
- Renewable resource potential validated against REZoning database
- Temporal analysis verified through statistical scenario methods

*For questions about specific data sources or methodology, refer to the
[VerveStacks Methods documentation](https://vervestacks.readthedocs.io/en/latest/).*

---
*Generated by VerveStacks Energy Model Processor*
