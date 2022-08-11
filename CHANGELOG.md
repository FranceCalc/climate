# Changelog
## 2.2
### Added
- CLM_calibration: Added another section to import additional data
- 1.4 Climate emissions:
    - Generates warnings for drought and flooding
### Changed
- 1.4 Climate emissions
    - Adjust Calibration to treat emissions not captured by EUCalc sectors
### Removed
- 1.4 Climate Emissions
    - Remove unneccessary second calibration for CO2e
### Fixed
- 1.4 Climate emissions
    - Fix missing cumulative emissions for rest of world

## 2.1
### Changes
- Calibration import now via GHG emissions import node
- Node 1.4 Climate emissions
    - General changes in workflow - calculation should now be much faster
    - Introduction of node checking if negative emission values are sensible
- Interface to agriculture: removes/introduces columns needed for the correct calibration to EuroStats database
- Interface to TPE: due to the changes in the interface with agriculture, some columns needed to be removed/introduced

## 2.0
### Added
- New lever "ems_after_2050" to handle different emissions trajectories
- New data files for ems_after_2050
- New data import node "clm_ems-after-2050"

### Changes
- Node 1.4 Climate emissions: new input port
- Interface to agriculture adjusted

## 1.9.5
### Changes
- Extended interface to Agriculture
- collapsing CO2e conversion into single node
### Removes
- Unneccessary nodes
### Fixes
- Calibration pathway now correctly produces calibrated and un-calibrated output

## 1.9
### Added
- Calculation of impacts in/by 2100 -> New section in 1.4 Climate Emissions
### Changes
- Node 1.4 Climate emissions:
    - Completely re-worked
    - updated calibration selection
    - CO2e calculation now per country
- Interface to TPE: columns for impacts


## 1.8
### Added
- New node CLM_calibration
- New port: calibration on node 1.4 Climate Emissions
- New data on crop yield for interface to agriculture

### Removes
- unneccessary data in the data folder
- Node clm_pre

### Changes
- Node CLM_tmp: changed to facilitate new agricultural data
- Node Level selection: port removed
- Node MatrixBuilder_Historical
- Update interface L2 for 1.4 Climate Emissions (integration of calibration update)
- Replace column aggregator nodes by tree merge nodes

### Fixes
- issues introduced with 1.7

## 1.7
### Added
- New data import node CLT_ems
- New data import node CLT_awi

### Changes
- additional column clt_emissions-CO2e[Mt] added to interface between 1.4 and TPE
- Edited node 1.4 Climate Emissions to incorporate workflow to calculate globa emissions and temperature changes up to 2100


## 1.6
### Added
- node 1.4 Climate Emissions (sub-module)
- node Update interface L2-GoogleSheet: Update 1.4 Climate Emissions
- interface 1.4 to 2.2 Transport
- interface 1.4 to 2.3 District Heating
- interface 1.4 to 3.1a Industry
- interface 1.4 to 3.1b Industry Ammonia
- interface 1.4 to 4.1 Land-use
- interface 1.4 to 4.3 Agriculture
- interface 1.4 to 4.5 Biodiversity
- interface 1.4 to 5.1 Electricity
- interface 1.4 to 5.2 Oil refinery
- interface 1.4 to pathway explorer
- interface 1.2 to 4.4 water

### Changes
- Update interface L2-GoogleSheet for 1.2 climate
  - new column creation nodes added
  - change of ports
    - port 1: 2.1 buildings
    - port 2: 5.1 Electricity
    - prot 3: 4.4 water
- Node Climate 1.2
  - new out port to 4.4 water

### Removes
- Interface 1.2 climate to pathway: This is now handled by 1.4 climate emissions

## 1.5
### Added
- Import climate data
- Interface to buildings

## 1.0
- Initial version, integrating all modules
