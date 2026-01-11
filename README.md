# NOTA: The Choice of Mugwumps?

## Description and Background: 
This project explores how NOTA votes in India impact the vote share of independent candidates. This repository consists of the following directories and files:

1. Publication/final_paper [Link](https://www.tandfonline.com/doi/abs/10.1080/02185377.2023.2265372): Contains introduction, literature review, methodology, results, conclusion and appendices. This document is the torso of the project. Interested reader should start here. A skimming reader should also start here but can skip literature review, methodology, and the appendices.     

2. Code : Documents codes used to produce figures and tables used in NOTA_Mugwumps.pdf. These files are for the meticulous reader who wants to verify the project results for him/herself. All codes are written in Python3.
   * 2.1. Code/01_input_dataprep.ipynb : Codes for cleaning the input data sourced from LokDhaba. Read Data/ancillary_files/pre_processing_data_meta.txt for more details.
   * 2.2. Code/02_fin_analysis.ipynb : Codes to reproduce the results given in the published paper.

3. Data/ancillary_files : Broadly, these are data files used in doc_codes.ipynb. In particular, it contains:
   * 3.1. cleanest_data.csv : Main input file containing pre_processed data used in Code/fin_analysis.ipynb

   * 3.2. pre_processing_data_meta.txt : Details about data source and initial data cleaning

   * 3.3. LokDhabaCodebook.pdf : Description of variables in the extracted, full dataset

   * 3.4. variables_description : Description of variables used and feature engineered in the dataset

   * 3.5. census_codes.csv : Contains census codes for various states used in assigning unique code to constituencies

   * 3.6. finding_salient.csv : This dataset is the result of subsetting processed data (cleanest_data.csv) to include only NOTA and independents. The DPS score can also be found in the dataset. In a nutshell, this dataset is the result of processing steps in Code/fin_analysis.ipynb and should be considered as the final dataset of this project.  

   * 3.7. lastpositionwins_perc.csv : Percentage times the last positions win pre and post NOTA. This dataset was generated using the pivot table feature on finding_salient.csv dataset and is used in the code to generate a bar chart in Code/fin_analysis.ipynb.

4. Analysis: Contains figures and regression results presented in the paper.