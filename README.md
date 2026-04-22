# Ensight Concentration Analysis

This code take the data table from different plate size and generates a color-coded table to quickly identify passing and failing wells based on a defined threshold.

## Requirement
For this code to work, we will need you to :
- Outfile from the Ensight machine in .csv format
- Upload the document on colab
- Libraries : pandas, matplotlib, numpy, string, glob

## Feature
- Read and automatically detects the plate size (6, 12, 24, 96, 384 well plates)
- Colors each well green if the concentration is above the threshold and red if it is below
- Outputs two lists of wells — passed and failed — for quick review
  - Modify threshold value to change the list output and color grading

## Usage
In the beginning of the code you have to establish the threshold. When this will be done you import you document on colab and run all the cells. Just like that you will have a color coded graph and a list off the wells that passed or failed.  
