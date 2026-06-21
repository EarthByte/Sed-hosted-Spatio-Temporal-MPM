# Sed-hosted-Spatio-Temporal-MPM
From Geodynamic Preconditioning to Mineral System Fertility: A Spatio-Temporal Analysis of Craton-Edge Sediment-Hosted Deposits

## Flowcharts of running notebooks for the sed-hosted STAMP Project:  

1-	Run  01_CalculateSpatialRelationships.ipynb. Craton boundary lines should be segmented by their azimuth (every 30 degree change)


2-	Assign plate ID to segmented craton boundaries in the GPlates software by looking at their movement based on the reconstruction model


3-	Assign plate ID to craton deposits in the GPlates software, the same as above


4-	Run Buffer_Paleo.ipynb; Reconstruct the craton boundaries and create a GeoJSON for each time step. Or reconstruct using gplates, export all time steps and then create a buffer in each time step. (Visually check in GPlates that everything is moving based on the anchor plate ID model.


5-	Run Movie_Paleo.ipynb notebook to double-check deposits and craton boundaries dance along with other topologies.


6-	Run 02_reconstruction_coregistration.ipynb to create backarc_coords and unlabelled_coords csv files.


7-	Run 02_Feature_Extraction_Deposits_Paleo.ipynb for deposit_coords and 02_Feature_Extraction_Target_Areas_Paleo.ipynb for unlabelled and backarc_coords. These will extract features for those files called *_data.


8-	Run 03_feature_analysis.ipynb


9-	Run 04_predictive_modelling.ipynb


10-	Run first part of 05_prospectivity_map.ipynb to create Points within Continental Landmasses (coastline_coords.csv)


11-	Run 02_Feature_Extraction_Target_Areas_Paleo.ipynb for coastline_coords.csv and create a coastline_data.csv


12-	Run the whole 05_prospectivity_map.ipynb 
