# Soil Carbon Prediction

Soil CO2 flux prediction using in-situ measurements via 

- Q10 Model
- Modified Q10 Model (with soil moisture)
- Random Forest regression with two variables
- Random Forest regression with 8 variables

## Data
The data used here includes:-

The daily soil CO2 flux data observed from LICOR's Automated Soil CO₂ Flux System over a dry deciduous forest system in India.

The variables soil water content (SWC), soil temperature (T_soil), atmospheric temperature (T_air), relative humidity (RH), incoming long-wave (RAD_lw) and short-wave radiation (RAD_sw), and soil heat flux (SHF) and the difference between atmospheric and soil temperatures (T_diff)

Hourly measurements of soil respiration, temperature, SWC, etc.
- `training.csv`: Data from 2015–2016
- `test_data.csv`: Data from 2018

## Models

1. **Q10**: Based on temperature sensitivity
2. **Modified Q10**: Adds moisture dependence
3. **Random Forest**: Machine learning models, one using temperature and SWC as variables , the other with 8 variabels

## Output

Final predictions are in gC m⁻² day⁻¹.

## Requirements

- R
- Libraries: dplyr, lubridate, ggplot2, caret, randomForest, caTools, ggpmisc

## Visualization

Plots show observed vs. predicted soil respiration and daily flux patterns.

