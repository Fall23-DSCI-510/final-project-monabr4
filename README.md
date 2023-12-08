# COVID-19 in Malaysia

Author's Note: Please read these docuements in order for to set up and understand the structure of the project and data --> (1)README.md (2)raw.txt (3)processed.txt 

## Introduction
 

The analysis focuses on understanding regional disparities in COVID-19 incidence rates across different states (13 states) in Malaysia and explores the impact of the pandemic on various regions in terms of cases and recoveries. It aims to uncover significant variations in how states have been affected. Additionally, the analysis takes a closer look at the correlation between population density in different states and the rate of COVID-19 transmission. By examining how states with diverse population densities have managed the spread of the virus, the analysis aims to find insights into the relationship between population density and the pandemic's impact in Malaysia.



## Research Questions



### Regional Disparities:

- How do COVID-19 incidence rates vary across different states in Malaysia?
- Are there significant disparities in the impact of the pandemic on various regions in terms of new cases and case recovery?

### Population Density and Transmission

- Is there a correlation between population density in different states and the rate of COVID-19 transmission?


## Datasets

The datasets collected include:

1. **Covid Cases by State:**
   - [API Documentation](https://covid-19.samsam123.name.my/api.html)

2. **Population of Malaysia:**
   - [API Documentation](https://documenter.getpostman.com/view/16605343/Tzm8GG7u)

3. **Malaysia ShapeFile:**
   - [Malaysia ShapeFile](https://cartographyvectors.com/map/1477-malaysia-with-regions)



## Project Structure

This data project is divided into three folders:

1. **Data**
    - **Processed:** The static datasets exported from raw data are located in this folder.
        - `final_covid_data.csv`
        - `final_raw_data.geojson`
        - `processed.txt`
    - **Raw:** API extraction and CSV conversions.
        - `exported_statis_csv_shapefile`
            - `STATES_CSV`
                - `All 13 state CSV Files `
            - `[static]malaysia_states.geojson`
            - `cleaned_population.csv`
        - `loading_shapefile.ipynb`
        - `loading_to_csv_ipynb`
        - `raw.txt`
        - `state_covid_data.csv`
        - `final_covid_data.csv`

2. **Results:**
    - `covid_percentage_by_state.png`
    - `covid_plot_with_diagnostics.png`
    - `graphing.ipynb`
    - `interactive_new_cases_by_state.html`
    - `recovered_rate_map.htl`
    - `results.txt`
    - `scatter_plot.png`

3. **Src:**
    - `__pycache__`
    - `utils`
- `README.md`
- `malaysia_covid.pdf`
- `requirements.txt`

  ## Dependencies

  - [pandas](https://pandas.pydata.org/) version 2.1.3
  - [matplotlib](https://matplotlib.org/) version 3.8.1
  - [seaborn](https://seaborn.pydata.org/) version 0.13.0
  - [scipy](https://www.scipy.org/) version 1.11.4
  - [geopandas](https://geopandas.org/) version 0.14.1
  - [plotly](https://plotly.com/) version 5.18.0
  - [folium](https://python-visualization.github.io/folium/) version 0.15.0
  - [statsmodels](https://www.statsmodels.org/stable/index.html) version 0.14.0

  
## Installation

To use this project, follow the steps below:

1. **Clone the Repository:**
   - Clone this repository to your local machine using the following command:

     ```bash
     git clone https://github.com/your-username/your-repository.git
     ```

2. **Navigate to the Project Directory:**
   - Change your current directory to the project's root folder:

     ```bash
     cd your-repository
     ```

3. **Data Loading:**
   - During the cleaning process, significant data manipulation and direct changes to the CSV files were made for merging data files.
   - When running the project, load static data from the following locations `graphing.ipynb`:
     - `data/processed/final_covid_data.csv`
     - `data/processed/final_rate_data.geojson`

Make sure to change the data directory to match your files in the `graphing.ipynb` file. 

4. **Run the Project:**
   - Execute the `graphing.ipynb`.

     Example command:

     ```bash
     python graphing.ipynb
     ```

5. **Explore the Results:**
   - After running the project, explore the generated results and visualizations.

 **Note:** Ensure that you have the necessary dependencies installed. You can install them using the following:

    ```bash
    pip install -r requirements.txt
    ```
## Python Version 


The analysis was conducted using Python version 3.11.5 (main, Aug 24 2023, 15:09:32) [Clang 14.0.0 (clang-1400.0.29.202)].

## Note 

Upon extraction from API and shapefiles, data cleaning was done in Data > Raw. Do NOT run the code in the "raw" folder. Manual data cleaning was performed. The final cleaned datasets are `final_covid_data.csv` and `final_raw_data.geojson` files. These files are used in the `graphing.ipynb` folder to compute the graphs. All the graphed results are located in the results folder. More information about how each folder is used can be found in `processed.txt`, `raw.txt`, and `results.txt`.

## Note 

The written report can be found in `malaysia_covid.pdf`.







