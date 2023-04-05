# Lending-Club-40k-R-Code

This code is performing data cleaning and imputation using the MICE (Multiple Imputation with Chained Equations) package in R for the Lending Club 40k dataset. The code sets the working directory, installs and loads necessary packages like dplyr, mice, and tidyr, reads in the original dataset, summarizes it, and then lowers the case of all job titles. The lower-cased dataset is then exported to a CSV file.

Further analysis is done in Excel and RapidMiner to remove incorrect job titles and outliers. The cleaned dataset is saved as LendingClub40k_corrected.csv. The corrected dataset is read in and the description and ID columns are subsetted and saved for future use. The desc and zip_code columns are dropped, and the remaining columns are summarized.

The code then checks for any missing values and looks at the missing data patterns in the in_data dataset. MICE is then used to impute the missing values with a random forest algorithm. The imputed dataset is then completed and checked for any remaining missing values. Finally, the imputed dataset is merged with the stored description and ID columns to create a clean dataset called Clean_dataset.
