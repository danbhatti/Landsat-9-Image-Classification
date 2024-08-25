# Landsat-9-Image-Classification

Landsat 9 Image Classification was conducted over a portion of the City of Lancaster and it's adjacent municipalities. Landsat data and Image Classification techinques were used to extrapolate four main land uses: water bodies, agriculture, forested, and built up areas. 


Landsat 8-9 OLI/TIRS C2 L1 imagery (LC09_L1TP_015032_20240716_20240717_02_T1) was downloaded for processing. IR Bands 1-7 were clipped to the area of interest and converted to reflectants using the packaged MTL file. 

Semi-Automatic Classification Plugin (SCP) was used to layer IR bands (e.g. 4-3-2 is natural color image) in order to highlight features like water bodies, healthy vegetation, etc. For each of water bodies, agriculture, and forested areas, 5 samples were chosen varying in their size and clarity. For built up areas, five samples were taken of suburban neighborhoods (dendritic street grid, mixed vegetation) and five samples were taken of urban areas with the aid of the Future Land Use and Transportation Map of the Lancaster County Comprehensive Plan (Places2040) and the Google Map satellite imagery to confirm land use intensity. Classification was done with Z-score input normalization using the Minimum Distance Algorithm. After classification we converted the map to HTML using qgis2web. All processing was done in QGIS.

