# TFTformer Dataset

This repository contains the datasets used in the paper:

> Ahmad Ahmad, Xun Xiao, Huadong Mo, and Daoyi Dong.  
> *TFTformer: A novel transformer based model for short-term load forecasting*.  
> International Journal of Electrical Power and Energy Systems, Vol. 166, 2025, 110549.  
> https://doi.org/10.1016/j.ijepes.2025.110549

## Dataset Description

The datasets cover electrical load and weather data from multiple geographical regions between **2015 and 2022**:

- **Belgium**: Load data from Elia TSO (hourly resolution)  
- **New Zealand**: Load data from the Electricity Authority (30-minute resolution)  
- **Australia**: Load data from AEMO  
  - New South Wales (NSW)  
  - Victoria (VIC)  
  - Queensland (QLD)  
  - South Australia (SA)  
  - Tasmania (TAS)  

Weather parameters (temperature, humidity, wind speed, wind direction, and cloud cover) were obtained from [Open-Meteo](https://open-meteo.com/).

All datasets were preprocessed to align load and weather data at an hourly resolution.

## Folder Structure

- `All Load Data/` contains xlsx files for each region.  
- Each xlsx file includes the following columns:
- `date`: local timestamp of the observation  
- `Year`: calendar year  
- `Month`: month number (1–12)  
- `Day of Month`: day of the month (1–31)  
- `Day of Week`: day of the week (1 = Monday, …, 7 = Sunday)  
- `hour`: hour of the day (0–23)  
- `Weekend / Public Holidays`: indicator (0 = weekday, 1 = weekend or public holiday)  
- `temp`: air temperature (°C)  
- `humidity`: relative humidity (%)  
- `precip`: precipitation (mm)  
- `windspeed`: wind speed (m/s)  
- `winddir`: wind direction (degrees)  
- `cloudcover`: cloud cover (%)  
- `Load`: electricity demand (MW) 

## Usage

You may use this dataset for academic and research purposes.  
If you use this dataset, please cite the paper listed above.

## Citation

Please cite:

```bibtex
@article{ahmad2025tftformer,
  title   = {TFTformer: A novel transformer based model for short-term load forecasting},
  author  = {Ahmad, Ahmad and Xiao, Xun and Mo, Huadong and Dong, Daoyi},
  journal = {International Journal of Electrical Power and Energy Systems},
  volume  = {166},
  pages   = {110549},
  year    = {2025},
  doi     = {10.1016/j.ijepes.2025.110549}
}
