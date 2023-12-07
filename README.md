
** COVID-19 in Malaysia **

Introduction: The analysis focuses on understanding regional disparities in COVID-19 incidence rates across different states (13 states) in Malaysia and explores the impact of the pandemic on various regions in terms of cases and recoveries. It aims to uncover significant variations in how states have been affected. Additionally, the analysis takes a closer look at the correlation between population density in different states and the rate of COVID-19 transmission. By examining how states with diverse population densities have managed the spread of the virus, the analysis aims to uncover insights into the relationship between population density and the pandemic's impact in Malaysia.

Research Questions:

Regional Disparities:

    -How do COVID-19 incidence rates carry across different states in Malaysia?
    -Are there significant disparities in the impact of the pandemic on various region in terms of case new cases and case recovery? 

Population Density and Transmission

    -Is there a correlation between population density in different states and the rate of COVID-19 transmission?


This data project can is divided into three folders: 

1. Data 
    - processed: The static data sets that were exported from raw data are loated in this folder 
        - final_covid_data.csv 
        - final_raw_data.geojson
        - processed.txt
    - raw: API extraction and CSV conversions 
        - exported_statis_csv_shapefile 
            -STATES_CSV
            - [static]malaysia_states.geojson
            - cleaned_population.csv
            - loading_shapefile.ipynb
            - loading_to_csv_ipynb
        - raw.text
        - state_covid_data.csv
        - final_covid_data.csv
2. results:
    - covid_percentage_by_state.png 
    - covid_plot_with_diagnostics.png
    - graphing.ipynb
    - interactive_new_cases_by_state.html
    - recovered_rate_map.htl
    - results.txt
    - scatter_plot.png
3. src:
    -__pycache__
    -utils
-README.md
-requirements.txt


Upon extraction from API and shapefiles, data cleaning was done in Data>Raw. Do NOT run the code in the "raw" folder. Manual data cleaning was done. The final cleaned data sets are "final_covid_data.csv" and "final_raw_data.geojson" file. These files are used in the "graphing.ipynb" folder to compute the graphs. All the graphed results are located in the results folder. More information about how each folder is used can me found in "processed.txt", "raw.txt", and "results.txt".








