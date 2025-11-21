# Analysis Scripts

The only script that this analysis makes use of is `analysis.ipynb`. This contains the 

## Note before running

Before running the cells in the notebook, ensure that you have properly loaded `data.tar.gz`. Steps for this in Google Colab are as follows

- Under the `files` section of the notebook, located on the left side of the screen choose the `upload` options
- Upload the `data.tar.gz` file from your computer that was either generated using the `tar` command, or simply from the provided dataset in this project (more information for preparing and setting up the dataset can be found [here](../datasets/README.md))
- The cells in the file are now able to run properly

## Steps

The script will first import and extract the files in `data.tar.gz`. In the notebook, a neew directory will be created called `datasets`. This directory will contain all of the raw csv files for each collected state.
The next step in the script will be to clean and combine all of the data into one main DataFrame. Step will include aggregations, column removing/renaming, removing missing data or imputing missing data and creating quartiles (binning data) for different metrics
Visuals are created in this script but the majaority of the visualzations are from the [Visualization Directory](../visualizations/README.md). The main purpose behind this script is to perform analysis on the data and prepare it for visualization in PowerBI.

## Output

One of the main outputs this script creates is a new file called `data.csv`. This is an important file for the [PowerBI Visualization](../visualizations/README.md) as it is the main source of data necessary for the visuals

Once all of the cells in the analysis are run, in the same `files` window where the original `data.tar.gz` was uploaded to, a new file called `data.csv` will also be present. This file can be downloaded and imported into PowerBI