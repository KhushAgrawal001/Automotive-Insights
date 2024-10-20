# Automotive Insights
*Sub: CAN300 Data Processing and Analysis*

## Overview
The **Automotive Insights** project focuses on the processing and analysis of the CAN300 dataset, which includes detailed telemetry and diagnostic information from vehicles. The goal is to un-nest the nested data structure, extract meaningful insights, and perform data profiling to understand vehicle performance and behavior.

## Project Structure
This repository contains the following key files:

- **Task 1 EDA**: 
  - *Jupyter Source File*: Analyzes the exploratory data and provides visualizations.
  - *Brave HTML Document*: A detailed report of the exploratory data analysis.

- **Task 1 Cleaning**: 
  - *Jupyter Source File*: Implements data cleaning and preprocessing steps to prepare the dataset for analysis.

- **CAN300 Un-nest Dataset Task**: 
  - *Jupyter Source File*: Handles the un-nesting of the dataset and extraction of key features.

- **Cleaned Data**: 
  - *File*: Contains the cleaned version of the CAN300 dataset ready for analysis.

- **yellow_tripdata_2023-05.parquet**: 
  - *PARQUET File*: An additional dataset used for comparative analysis.

- **Successfully Running Jobs**: 
  - *JPG File*: A snapshot of the successfully executed jobs and processes.

- **Nested Data with Masked VINs**: 
  - *Compressed File*: Contains nested data with masked VINs for privacy.

## Key Components
The dataset is structured with several important components, including:
- **Headers**: Metadata about the dataset, including keys like `Masked-VIN`, `dispatchModelType`, and `ModelYear`.
- **GPS Data**: Contains latitude, longitude, and other telemetry information.
- **CAN Information List**: Provides detailed diagnostic signals relevant to vehicle performance.
- **Outside Use Data**: Additional telemetry data recorded under various conditions.

## Data Profiling
The project implements data profiling techniques to extract distinct values for the following signals:
- Signal labels (e.g., label_51F)
- Masked-VIN
- Dispatch model type (Katashiki)
- Model Year
- Vehicle Name (Model)

Aggregations are performed based on date, month, year, Model Year, and VIN to generate insights and trends from the data.

## Requirements
- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib / Seaborn (for visualizations)
- Other libraries as needed

## Getting Started
To get started with the project:
1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/Automotive-Insights.git
2. Navigate to the project directory:
   ```bash
   cd Automotive-Insights
3. Open the Jupyter Notebook for data analysis:
   ```bash
   jupyter notebook
