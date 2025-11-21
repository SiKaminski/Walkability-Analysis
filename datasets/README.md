# Datasets

## Preparation

All data is contained in this directory. The data is split into groups by state, with subdirectories for each state named by its abriviation (AZ, NY, CA, etc...)

To import the data into a Google Colab session, the first step necessary is to compress the data into a tar archive named `data.tar.gz`. This can be done using the following command in the root directory of the repository

```bash
tar -czvf data.tar.gz datasets/
```

Alternatively, the provided `data.tar.gz` file in this directory can be used as it will be the most up to date with the data in this repository

## Data Format

All data is collected from PolicyMap using the web interface. Ideally the data should be collected via API calls to ensure better reproducability but I did not want to spend too much time attempting to understand the PolicyMap API for this project. In the future if I revist this project I would like to spend more time on data collection. Each state file in this directory contains the following files which can be found in PolicyMap in the following locations

| File name                        | Location (PolicyMap)                                                                                          |
|----------------------------------|-----------------------------------------------------------------|
| distance_to_nearest_transit      | QOL > Transportation > Public Transit > Distance to nearest stop                                              |   |   |   |
| jobs_within_45_min_by_car        | QOL > Transportation > Job and Worker Accessibility > Jobs within 45 min > Auto Travel                        |
| jobs_within_45_min_by_transit    | QOL > Transportation > Job and Worker Accessibility > Jobs within 45 min > Transit Commute                    |
| national_walkability_index       | QOL > Transportation > Walkability > NWI                                                                      |
| pedestrian_oriented_road_density | QOL > Transportation > Transportation Infra > Road Network Density > Pedestrian-oriented Road Network Density |
| population_density               | Demographics > Population > Population Density                                                                |
| total_road_density               | QOL > Transportation > Transportation Infra > Road Network Density > Total Road Network Density               |
| vehicles_per_household           | QOL > Trnasportation > Vehicles per Household > Avg                                                           |
| pct_drove_to_work                | QOL > Transportation >  Mode of Transportation to Work > Drive                                                |
| pct_public_transit_to_work       | QOL > Transportation >  Mode of Transportation to Work > Public Transit                                       |
| pct_bike_to_work                 | QOL > Transportation >  Mode of Transportation to Work > Bicycle                                              |
| pct_walk_to_work                 | QOL > Transportation >  Mode of Transportation to Work > Walk                                                 |
| per_capita_income                | Income & Spending > Income > Per Captia                                                                       |