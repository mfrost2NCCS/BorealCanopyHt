# BorealCanopyHt
# Melanie Frost
# 5/1/2023

Files for the Boreal Canopy Height 
1. "Train_RF_model_Apr2023v2.ipynb"
  - Trains and creates RF model for predicting canopy height int he Boreal region using ATL08. Incoudes perm
  - Shows histogram of caopy heights
  - Includes permafrost as an input variable
  - includes ranked permuation importance as RF output

2. "Prediction_Apr2023v2.ipynb"
  - Loads model created in previous step
  - Applies model on current bioclimate and shows prediction. Saves as raster
  - Applies models on future bioclims from CMIP6: 
    - 2021-2040
    - 2061-2080
    - 2081-2100
  - and from scenarios
    - ssp126
    - ssp245
    - ssp370
    - ssp585
  - Creates rasters of predictions for each year x scenario x GCM
  - Creates difference of prediction from current for each year x scenario X GCM
  - Can create scatter plots between scenarios
  - Create pixel-by-pixel median raster for each year x scenario
 
3. "Boreal_median_maps.ipynb"
  - Show raaster of current prediction
  - Show faceted maps for prediction/difference (columns), and scenario (row)
  - Show faceted histograms for prediction/difference (columns), and scenario (row)
