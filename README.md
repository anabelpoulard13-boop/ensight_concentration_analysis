# Ensight Concentration Analysis
This script was created to simplify the analysis and estimation of concentration in an experiment. It takes raw absorbance data from an Ensight machine in `CSV` format and determines the concentration function using two variables defined at the beginning of the code.

## Requirement
For this code to work, we will need you to :
- A file from the Ensight machine in `.csv` format
- Upload the document on colab
- Libraries : pandas, matplotlib, numpy, string, glob, os
- Define a:

`blank_well` : the concentration of that well is always 0

`sample_well` : a well that will have a precalculated concentration

`sample_concentration` : concentration of that sample

## Feature
- Reads and automatically detects the plate size (6, 12, 24, 96, 384-well plates)
- Generates a data frame with only relevant data from the file
- Calculates the slope and y-intercept to build a function (y-axis: absorbance, x-axis: concentration)
- Applies the calculation to all cells in the data frame (concentration table)
- Removes all unusable data and generates a plot of the function using two points
- Generates a heatmap with a color scale (darker colors for high concentration, lighter colors for low concentration)
- Outputs: an Excel file with the cleaned data and a CSV list of all well positions with their corresponding concentrations

## Usage
At the start of the code, you need to define the three variables. Then, upload your document to Colab and run all the cells. This will generate a data frame with only the relevant concentrations, along with a heatmap to visualize the data. You will also get a file in Colab named `result` which includes an Excel sheet of the data table and a `CSV` list of all the well positions with their concentrations.
