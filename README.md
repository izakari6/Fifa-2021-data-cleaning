FIFA 2021 DATA CLEANING CHALLENGE

INTRODUCTION
One of the challenging tasks for every data analyst is cleaning and preparing data for further analysis. When data is not clean of irregularities and standardised, it becomes impossible to analyse and make visualisations. 
The focus of this project was to clean a messy FIFA dataset and prepare it for further analysis. The dataset was sourced from Kaggle which had 18979 rows and 77 columns. The entire data cleaning process was done with Python (Jupyter Notebook).

CONTENT
After loading the raw data file into Jupyter notebook, various functions (df.shape, df.describe(), df.info(), df.isnull(), df.duplicated(), etc) was implemented to identify all data columns which needed to be cleaned. It was discovered that, some data columns were irrelevant, so there was a need to drop them. Such columns were:
•	Photourl
•	Playerurl
•	Name
•	Loan End Date
Also, on further explorations of the dataset, some other columns, where detected to have some anomalies such as multiple information in the same cell, inappropriate data types, Na values and Null cells, and special characters. Such columns were:
•	Club
•	Contract
•	Positions 
•	Height
•	Weight
•	Value
•	Joined
•	Wage
•	Release Clause
•	W/F
•	Sm
•	IR
•	Hits

The cleaning process integrated standardization of unit of measurement for the (Height as cm, Weight as lbs) and also replacing all numeric abbreviations (Thousand as K, Million as M, and € as Euro) from data in the (Value, Wage, and release Clause) columns.
Columns such as Club, W/F, IR, and SM had special characters (\n, ★) which need to be removed.
The column Contract had mixed information (dates, free, and on loan) which was further sorted into (Contract start, Contract end, and Contract type) columns. Afterwards the Contract column was dropped since it would not be need again.
Finally, some columns were renamed so that it can better describe its content.

CONCLUSION & RECOMMENDATIONS
Getting involved with the data cleaning challenge has really exposed me to new techniques on how to use python for data analytics. A lot has been learnt from a community of aspiring data analyst. One recommendation I can make is that, as a data analyst it is important to make further research on the niche of the dataset you are working on.

Thank you for your time.
Comments and remarks are welcomed.


