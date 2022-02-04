<b> NOTE: This project is a current work in progess. </b>

<b> I spent 35+ hours and about 1 month on this project. </b>
 
# Chicago-COPA-Dataset

The Dataset used in this project can be found at: https://www.kaggle.com/chicago/chicago-copa-cases/version/20

# Quick Description of Dataset

1. Each row is a complaint by a person(s) submitted to an internal review board with an allegation that a police officer mistreated them in some way. 
2. The data is from the Chicago Police Department

# Files Description

NOTE: This project is a work in progress.

This project consists of two files.

1. Chicago COPA - Data Cleaning.ipynb -> This notebook focuses on cleaning and transforming raw data into more useful forms. Unfortunately, some columns in this dataset are extremely dirty and I had to perform extensive data cleaning.

2. Chicago COPA - Analysis.ipynb -> This notebook performs an extensive analysis of the races of police officers and complainants.

3. no_bia_with_officer_information.csv -> Cleaned dataset with all nesscessary columns.

4. copa-cases-summary.csv -> Original Dataset.

# Summary of Findings

<font size="8"> <b> CORRELATION STUDY: </b> </font>

      1. The more black complainants are involved, the greater number of black police officers are involved.
      2. The more Hispanic complainants are involved, the greater number of Hispanic police officers are involved.
      3. The more white complainants are involved, the greater number of white police officers are involved.

      All three have a very weak correlation but are statistically significant 
      due to extremely small p-values. 
      
      Further improvement in methodologies and further study is required to yield more evident results.

![image](https://user-images.githubusercontent.com/40840760/149868620-1cb3279e-ea3b-4cae-9ebe-f286dd806032.png)

![image](https://user-images.githubusercontent.com/40840760/149868710-083c25e9-42dd-492f-8b20-8bff387ce939.png)

![image](https://user-images.githubusercontent.com/40840760/150880671-64621cd2-bbc4-4323-b12e-19833026b624.png)

![image](https://user-images.githubusercontent.com/40840760/150880717-91d10464-bc95-4a11-8aaf-a8c026822157.png)


 <font size="8"> <b> GENERAL FACTS: </b> </font>

      1. Approximately 94% of complaints involve 3 or less police officers
      2. 66% of complaints only involve 1 police officer.
      3. 22% of complaints involve 2 police officers.
      4. 11569 complaints inolve only 1 police officer.
      5. 3867 complaints involve 2 police officers.
      6. 1034 complaints involve 3 police officers.

![image](https://user-images.githubusercontent.com/40840760/149868844-d0ed4c87-1a15-4b6c-9b38-f0ee9008f601.png)

-------------------------------------------------------------------------------------------------------------------------------------

<p align=center> <font size="8"> <b> COMPLAINANT/OFFCIER RACE STUDY: </b> </font> </p>
 
This section aims to analyze the races of police officers and races of complainants involved in mistreatment allegations.

Specifically, this section attempts to answer the following question: Are a particular race of complainants more likely to file a complaint against a particular race of police officers?

For example: Are whites more likely to file a complaint against Hispanic police officers?



Below is a graph of relative rates of how much each complainant race files a complaint against BLACK police officers.

Findings:

1.	Black complainants have the highest rates of reporting other black police officers. 29% of police officers reported by the Black complainants are black police officers.
2.	Hispanic complainants have the lowest rates of reporting other black police officers. (no data for natives)
3.	White complainants have the second-lowest rates of reporting other black police officers.






      
      

