# Suicide Analysis Data Mining Project

``` mermaid
flowchart TD
    subgraph "Project Documentation"
        Readme["Project Overview and Objectives (README.md)"]:::doc
    end

    CSVData["CSV Data Source (suicide_rates_1990-2022.csv)"]:::data
    Notebook["Jupyter Notebook (Suicide_Analysis_DataMining.ipynb)"]:::notebook

    subgraph "Data Analysis Pipeline"
        DataLoading["Data Loading (pandas)"]:::process
        Preprocessing["Preprocessing"]:::process
        EDA["Exploratory Data Analysis (pandas,Matplotlib,Seaborn)"]:::process
        ML_DM["Machine Learning/Data Mining (scikit-learn)"]:::process
        Visualization["Visualization & Insights"]:::process
    end

    Readme -->|"informs"| Notebook
    CSVData -->|"ingests"| Notebook
    Notebook -->|"executes"| DataLoading
    DataLoading -->|"cleans"| Preprocessing
    Preprocessing -->|"explores"| EDA
    EDA -->|"models"| ML_DM
    ML_DM -->|"visualizes"| Visualization

    click Readme "https://github.com/binduyerra/suicide_analysis_data_mining/blob/main/README.md"
    click CSVData "https://github.com/binduyerra/suicide_analysis_data_mining/blob/main/suicide_rates_1990-2022.csv"
    click Notebook "https://github.com/binduyerra/suicide_analysis_data_mining/blob/main/Suicide_Analysis_DataMining.ipynb"

    classDef data fill:#ffcccc,stroke:#cc0000,stroke-width:2px;
    classDef notebook fill:#ccffcc,stroke:#006600,stroke-width:2px;
    classDef process fill:#ccccff,stroke:#0000cc,stroke-width:2px;
    classDef doc fill:#fff0b3,stroke:#ffaa00,stroke-width:2px;
 ```



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
