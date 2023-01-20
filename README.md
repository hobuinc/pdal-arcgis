# PDAL Examples Inside ArcGIS Pro

To use PDAL inside ArcGIS pro, a combination of `conda-forge` packages in an ESRI conda environment needs to be maintained, to simplify the setup, a conda specfile is provided that can be used to create the conda enviornment necessary to run a recent version of PDAL.

## Setup

1. Clone the repository.


1. Open the ArcGIS Pro Python Command prompt, and run the following command, where `specfile.txt` is the path to the specfile in this repository.

    ```doscon
    (arcgispro-py3) C:\Users\ogi\AppData\Local\Programs\ArcGIS\Pro\bin\Python\envs\arcgispro-py3>conda create \
    --name pdal-arcgis \
    --file specfile.txt
    ```

1. Open ArcGIS Pro, go to the Package Manager tab, click on the gear icon and browse to the newly created "pdal-arcgis" environment. Upon selection, activate it.

1. Restart ArcGIS Pro
1. Go to Insert, Add Notebook, and select `pdal_examples.ipynb` that is in this repo.
