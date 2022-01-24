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


 <font size="8"> <b> RACE MAJORITY STUDY: </b> </font>
 
<b>NOTE: THIS SECTION IS A WORK IN PROGRESS.                  </b>
 
The race majority study aims to analyze the races of police officers being reported by complainants in cases where most complainants are of one race. This type of analysis is performed to answer the following question:

Is a specific race of complainants more likely to file a report against a particular race of police officer. For example, are white complainants more likely to file a complaint against Hispanic police officers? If so, in what types of mistreatment allegations?

The graphs below show the distribution of police officer races where most complainants are black.

![image](https://user-images.githubusercontent.com/40840760/149868933-0f00ff03-58e0-4d5c-885d-7898d253b46a.png)

The graph below shows the relative frequency of police officers' races where most complainants are black.

![image](https://user-images.githubusercontent.com/40840760/149868966-25e84b39-99a9-46bc-9eaf-bfd8bbf34f71.png)




      
      

