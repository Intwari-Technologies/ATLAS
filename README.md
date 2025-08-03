# ATLAS v0.1: a prototype global landslide forecasting framework using dual-architecture deep learning

## overview
we used a duak-branch 3D CNN architecture to separately process static terrain features and and dynamic environmental conditions to predict landslides with an AUC-ROC of 0.731
we took 6 different streams of data from google earth engine to contextualize a filtered and cleaned dataset of landslide events sourced from NASA's COOLR and the University of Sheffield's GFLD datasets
the model accepts inputs as 4d tensors encoding time, width, height, and channels, looking at 12 time intervals of 6 hours to cover 3 days of antecedent data while also considering a 15x15 area of 90x90m pixels around a location
planning to update this model for greater accuracy and accessibility in the coming weeks and months. this version of ATLAS is not intended for use as an emergency measure.

## requirements
see requirements.txt

## citations
1. Kirschbaum, D.B., Stanley, T., & Zhou, Y. (2015). Spatial and temporal analysis of a global landslide catalog. Geomorphology, 249, 4-15. doi:10.1016/j.geomorph.2015.03.016
2. Kirschbaum, D.B., Adler, R., Hong, Y., Hill, S., & Lerner-Lam, A. (2010). A global landslide catalog for hazard applications: method, results, and limitations. Natural Hazards, 52, 561-575. doi:10.1007/s11069-009-9401-4
3. Froude, M. J. and Petley, D. N.: Global fatal landslide occurrence from 2004 to 2016, Nat. Hazards Earth Syst. Sci., 18, 2161–2181, https://doi.org/10.5194/nhess-18-2161-2018, 2018.
4. Saha, S., et al. 2011, updated daily. NCEP Climate Forecast System Version 2 (CFSv2) 6-hourly Products. Research Data Archive at the National Center for Atmospheric Research, Computational and Information Systems Laboratory. https://doi.org/10.5065/D61C1TXF. Accessed 13 Jul 2025.
5. 'Linke, S., Lehner, B., Ouellet Dallaire, C., Ariwi, J., Grill, G., Anand, M., Beames, P., Burchard-Levine, V., Maxwell, S., Moidu, H., Tan, F., Thieme, M. (2019). Global hydro-environmental sub-basin and river reach characteristics at high spatial resolution. Scientific Data 6: 283. DOI:10.1038/s41597-019-0300-6.'
6. Lehner, B., Verdin, K., Jarvis, A. (2008): New global hydrography derived from spaceborne elevation data. Eos, Transactions, AGU, 89(10): 93-94.
7. Theobald, D. M., Harrison-Atlas, D., Monahan, W. B., & Albano, C. M. (2015). Ecologically-relevant maps of landforms and physiographic diversity for climate adaptation planning. PloS one, 10(12), e0143619
8. Tomislav Hengl. (2018). Soil bulk density (fine earth) 10 x kg / m-cubic at 6 standard depths (0, 10, 30, 60, 100 and 200 cm) at 250 m resolution (Version v02) [Data set]. Zenodo. 10.5281/zenodo.1475970
9. NASA JPL (2020). NASADEM Merged DEM Global 1 arc second V001 [Data set]. NASA EOSDIS Land Processes DAAC. Accessed 2020-12-30 from doi:10.5067/MEaSUREs/NASADEM/NASADEM_HGT.001
