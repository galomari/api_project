
GDP Comparison Analysis

Overview

This project provides an analysis of GDP data for various countries across different continents for the years 2022 and 2023. The goal is to compare the GDP values to observe economic growth or decline during this period.

Data

The dataset includes GDP data for the following countries:

United States
China
Japan
Germany
India
United Kingdom
France
Italy
Canada
Brazil
Each country’s data is categorized by continent and includes GDP values for the years 2022 and 2023.

Data Columns

Country: The name of the country.
Continent: The continent where the country is located.
GDP (Million USD): The GDP value for the year 2023 in million USD.
Year 2023: The year corresponding to the 2023 GDP value.
GDP 2022: The GDP value for the year 2022 in million USD.
Year 2022: The year corresponding to the 2022 GDP value.
Data Transformation

The columns Continent and GDP 2023 have been renamed to Country and GDP (Million USD) respectively for clarity and ease of understanding.

Usage

Prerequisites
Ensure you have the following Python packages installed:

pandas
Steps
Load the Data:
Load the provided dataset into a pandas DataFrame.

Rename Columns:
Rename the columns for better readability using the following code snippet:

python
Copy code
import pandas as pd

# Assuming the DataFrame is named df
df = pd.DataFrame({
    "Country": ["United States", "China", "Japan", "Germany", "India", "United Kingdom", "France", "Italy", "Canada", "Brazil"],
    "Continent": ["Americas", "Asia", "Asia", "Europe", "Asia", "Europe", "Europe", "Europe", "Americas", "Americas"],
    "GDP 2023": [26854599, 19373586, 4409738, 4308854, 3736882, 3158938, 2923489, 2169745, 2089672, 2081235],
    "Year 2023": [2023] * 10,
    "GDP 2022": [25462700, 17963171, 4231141, 4072192, 3385090, 3070668, 2782095, 2010432, 2139840, 1920096],
    "Year 2022": [2022] * 10
})

# Renaming the columns
df.rename(columns={'Continent': 'Country', 'GDP 2023': 'GDP (Million USD)'}, inplace=True)
Analyze Data:
Perform various analyses, visualizations, or further transformations as required.

Future Work

Include additional economic indicators such as inflation rate, unemployment rate, etc.
Extend the analysis to more years to observe long-term trends.
Implement visualization dashboards using tools like PowerBI or Tableau.
License

This project is licensed under the MIT License.

Contact

For any questions or suggestions, please contact Ghaith M. Alomari at gaeth466@gmail.com.

