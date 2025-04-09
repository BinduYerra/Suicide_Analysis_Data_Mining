# Suicide Analysis Data Mining Project

``` mermaid
flowchart TD
    %% Main Pipeline
    DS["Raw Data Input (CSV)"]:::dataSource
    NB["Analysis Notebook"]:::notebook
    DOC["Documentation & Overview"]:::dataSource

    DS -->|"ingested by"| NB

    subgraph "Pipeline Steps"
        DI["Data Ingestion & Loading"]:::processing
        DC["Data Cleaning & Preprocessing"]:::processing
        EDA["Exploratory Data Analysis"]:::processing
        DV["Data Visualization"]:::output
        ML["Machine Learning/Data Mining"]:::processing
    end

    NB --> DI
    DI -->|"processes"| DC
    DC -->|"transitions"| EDA
    EDA -->|"feeds"| DV
    DV -->|"triggers"| ML

    NB -->|"references"| DOC

    %% Click Events
    click DS "https://github.com/binduyerra/suicide_analysis_data_mining/blob/main/suicide_rates_1990-2022.csv"
    click NB "https://github.com/binduyerra/suicide_analysis_data_mining/blob/main/Suicide_Analysis_DataMining.ipynb"
    click DOC "https://github.com/binduyerra/suicide_analysis_data_mining/blob/main/README.md"

    %% Styles
    classDef dataSource fill:#ADD8E6,stroke:#0000FF,color:#000000,font-family:Arial,font-size:14px;
    classDef notebook fill:#D3D3D3,stroke:#808080,color:#000000,font-family:Arial,font-size:14px;
    classDef processing fill:#F4A460,stroke:#FF8C00,color:#000000,font-family:Arial,font-size:14px;
    classDef output fill:#90EE90,stroke:#008000,color:#000000,font-family:Arial,font-size:14px; ```



# Overview
This project contains a Jupyter notebook Suicide_Analysis_DataMining.ipynb that performs a detailed data mining analysis on global suicide rates. It aims to uncover patterns, trends, and correlations that may help understand the underlying factors influencing suicide rates worldwide.

# Objectives
To analyze global suicide data to identify key demographic and socio-economic factors.

To utilize data mining techniques such as clustering, association rule mining, and predictive modeling.

To provide insights that could assist in formulating strategies to reduce suicide rates.

# Data Source
The dataset used in this analysis includes data on suicide rates from various countries, spanning several years. Data attributes include age, gender, country, year, and socio-economic indicators.

# Tools and Libraries Used
Python: For scripting and running data analysis.

Pandas and NumPy: For data manipulation and numerical calculations.

Matplotlib and Seaborn: For data visualization.

Scikit-learn: For implementing machine learning algorithms.
