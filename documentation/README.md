# Capstone

## Data

All data is contained in this directory. The data is split into groups by state, with subdirectories for each state named by its abriviation (AZ, NY, CA, etc...)

To import the data into a Google Colab session, the first step necessary is to compress the data into a tar archive named `data.tar.gz`. This can be done using the following command in the root directory of the repository

```bash
tar -czvf data.tar.gz datasets/
```

Alternatively, the provided `data.tar.gz` file in this directory can be used as it will be the most up to date with the data in this repository

More information about the datasets can be found in the [Datasets Documentation](../datasets/README.md)

## Analysis

The original analysis for this project was developed in [Google Colab](https://colab.research.google.com/) and the python script for the analysis can be found in the [Scripts Directory](../scripts/README.md)

## Visualization

The data required for the PowerBI visualization is outlined in the [Visualization Documentation](../visualizations/README.md)