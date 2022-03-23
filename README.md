# IAS Classification
Python (Jupyter Notebook) scripts used in "Nuijten and Coops (2022) Invasive alien species monitoring using multi-camera imagery in open boreal forests"


The repository includes the following Jupyter Notebooks.

1. Preprocessing_scale_rasters.ipynb
2. Preprocessing_stacking_rasters.ipynb
3. Preprosessing_clip_and_raster2points.ipynb
4. Preprosessing_split_samples.ipynb
5. SVM_classification_and_performance.ipynb

Image processing needs to be peformed in Agisoft Metashape beforehand, resulting in two orthomosaics with near-centimeter accurate alignment. You can scale, stack and clip (by field transect) orthomosaics, as well as convert them to points using the first three scripts. Then you need to select target and absent points for both species. We used the Editor tool in ArcGIS Pro, however open-source tools like QGIS can be used as well. Splitting target and absent-class samples by 2x2 m2 field quadrat and 2x2 cm2 fishnet grid, can be performed using script 4. Finally SVM is performed using script 5, including synthetic undersampling (k-means), gridsearch, and classification performance assessment.

I haven't annotation all steps in the code properly, so feel free to contact me if code is unclear or if you are not able to implement it.

Thank you,
Rik
