<b> NOTE: This project is a current work in progess. </b>

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

<p align=center> <font size="8"> <b> CORRELATION STUDY: </b> </font> </p>

      1. The more black complainants are involved, the greater number of black police officers are involved.
      2. The more Hispanic complainants are involved, the greater number of Hispanic police officers are involved.
      3. The more white complainants are involved, the greater number of white police officers are involved.
      4. The more Hispanic complainants are involved, the lesser number of black police officers get involved.
      5. The more white complainants are involved, the lesser number of black police officers get involved.

      All five have a weak correlation but are statistically significant 
      due to extremely small p-values. 
 
![image](https://user-images.githubusercontent.com/40840760/152620963-3db026bd-9fd0-466a-8347-c7192ab3e4f9.png)

The more black complainants are involved, the greater number of black police officers are involved.
SpearmanrResult(correlation=0.25080355222253364, pvalue=1.4710339851136814e-158)

![image](https://user-images.githubusercontent.com/40840760/152615114-3060b0cf-ca79-46e5-a793-2b5fd5f07649.png)

The more Hispanic complainants are involved, the greater number of Hispanic police officers get involved.
SpearmanrResult(correlation=0.1733228608617746, pvalue=1.7935709043535574e-75)

![image](https://user-images.githubusercontent.com/40840760/152615146-d68aa539-26ae-4dc0-a9ad-e72719235c2c.png)

The more white complainants are involved, the greater number of white police officers get involved.
SpearmanrResult(correlation=0.15826798777912449, pvalue=4.4056382291695707e-63)

![image](https://user-images.githubusercontent.com/40840760/152615174-2e978d98-a16e-4d2b-a5d4-21d25c223c1d.png)

The more Hispanic complainants are involved, the lesser number of black police officers get involved.
SpearmanrResult(correlation=-0.17425534481387886, pvalue=2.8009639768461656e-76)

![image](https://user-images.githubusercontent.com/40840760/152616483-db122553-3ef4-4c79-94f3-ff3fb17b3f2d.png)

The more white complainants are involved, the lesser number of black police officers get involved.
SpearmanrResult(correlation=-0.15190808500268096, pvalue=3.349564974999276e-58)

![image](https://user-images.githubusercontent.com/40840760/152616498-9d8e97ad-eb3c-45f6-91ca-fc13b3e4290c.png)

------------------------------------------------------------

<p align=center> <font size="8"> <b> Analysis of Races of Complainants Involved In Mistreatment Allegations </b> </font> </p>

This section analyzes the race distribution of complainants involved in police mistreatment allegations.

First, let us look at the race distribution from allegations between 2008 to 2018. About 71% of complainants are black. While Hispanics make up 14.4% of complainants and Whites, make up 10.4% of complainants. The other 4.2% are of other or unknown races.

![image](https://user-images.githubusercontent.com/40840760/156479211-42aa99b5-da83-4a99-b17e-980b91a4db8d.png)

As you can see above, blacks are disproportionately represented as complainants. Is it possible that Chicago is primarily black? This would explain the results. However, this is not the case. In 2016, 29.3% of people living in Chicago were black, yet blacks make up 70.5% of all complainants in mistreatment allegations.

Now the question is: have blacks always made up the majority of complainants?

To analyze this, I created a graph below.

The graph below shows the percentage contribution of each complainant race between 2008 and 2018. The chart is interpreted like this: in 2010, approximately 18% of complainants were Hispanic.  

![image](https://user-images.githubusercontent.com/40840760/156479304-84c4af6b-d5cb-42af-8e87-29eb683b226f.png)

From 2008 to 2018, blacks make up the majority of complainants by a substantial margin. In 2011, the percentage contribution of black complainants was at its peak when 73.9% of complainants were black.

Moving on to analyzing the percentage contribution of Native, Asian, Hispanic, and Whites. I created the graph below, similar to the graph above, except Blacks are excluded in the chart.

![image](https://user-images.githubusercontent.com/40840760/156479374-23c8d428-8afd-4dae-801c-a6bff68c750d.png)

Interestingly, the percentage of complainants that are Natives, Asians, Hispanics, and Whites has remained stable over 10 years. However, a larger percentage of complainants have Unknown races. The percentage contribution of complainants of Unknown races has increased from 1.03% in 2011 to 6.19% in 2018.

So far, I have analyzed the race distribution of complainants in two ways,  on a year-by-year basis and an aggregate level from 2008 to 2018. My analysis did not include taking into account the type of mistreatment allegation. There are 20 types of mistreatment allegations in the dataset. A list of mistreatment allegations is provided by the image below.

![image](https://user-images.githubusercontent.com/40840760/156479412-06dac887-e69c-496c-982b-4ba576160c88.png)

I will analyze the race distribution of complainants on a year-by-year basis grouped by the mistreatment allegation.

For example, I will analyze Excessive Force allegations. This is the most common type of allegation

![image](https://user-images.githubusercontent.com/40840760/156479452-9da45882-e05d-4a5d-8f1b-8e4875b7cf67.png)

For Excessive Force complaints, blacks make up the largest percentage of complainants by a huge margin, with an average percentage of 70.9% between 2008 and 2018.

![image](https://user-images.githubusercontent.com/40840760/156479478-30f30456-d146-4a81-84ed-972d5e48ffdc.png)

Looking more closely into the trend for black complainants, there was a massive spike in the percentage of black complainants for excessive force complaints. The percentage in 2017 was 66%, and in 2018, the percentage was 75%, the highest percentage value between 2008 to 2018.

Now, I will analyze the percentage of complainants that are other races involved in excessive force complaints.

![image](https://user-images.githubusercontent.com/40840760/156479506-7d78acc4-737e-447e-b798-b8f504237c3b.png)

We can see that the most frequent excessive force complainants are in the following order: Blacks, Hispanics, Whites, Unknown, Asians, and Natives. The percentage of complainants that are non-black have remained stable from 2008 to 2017. However, in 2018, there is a massive shift in the percentage frequency for all complainant races. For example, the percentage of complainants that are Whites have decreased from 13% to 6.43%. Similarly, percentage of complainants are of Unknown races have increased from 2.64% to 5.6%. 

------------------------------------------------------------

<p align=center> <font size="8"> <b> COMPLAINANT/OFFICER RACE STUDY: </b> </font> </p>
 
This section aims to analyze the races of police officers and races of complainants involved in mistreatment allegations.

Specifically, this section attempts to answer the following question: Are a particular race of complainants more likely to file a complaint against a particular race of police officers?

For example: Are whites more likely to file a complaint against Hispanic police officers?


<b> Below is a graph of relative rates of how much each complainant race files a complaint against BLACK police officers. </b>

Findings:

1.	Black complainants have the highest rates of reporting other black police officers. 29% of police officers reported by the Black complainants are black police officers.
2.	Hispanic complainants have the lowest rates of reporting other black police officers. (no data for natives)
3.	White complainants have the second-lowest rates of reporting other black police officers.

![image](https://user-images.githubusercontent.com/40840760/152613661-c8f9e350-1403-4283-8954-22cf31f12f40.png)

<b>Below is a graph of relative rates of how much each complainant race files a complaint against HISPANIC police officers.</b>

Findings:
1.	Hispanic complainants have the highest rates of reporting other Hispanic police officers. 36% of officers reported by Hispanic complainants are Hispanic police officers.
2.	Native complainants have the lowest rates of reporting Hispanic police officers, around 8.3%.
3.	Whites, Unknowns and Blacks all have the same rates of filing a complaint against Hispanic police officers.

![image](https://user-images.githubusercontent.com/40840760/152613717-37e2bf3d-6e7d-44d8-9f85-90cf0ea47222.png)

<b> Below is a graph of relative rates of how much each complainant race files a complaint against ASIAN police officers. </b>

Findings:

1.	Native complainants have the highest rates of filing complaints against Asian police officers. 25% of officers reported by Native complainants are Asian police officers.
2.	Asian complainants come in second place for filing complaints against Asian police officers. 9.9% of officers reported by Asian complainants are Asian police officers.
3.	All other races have similar rates of filing a complaint against Asian police officers.

![image](https://user-images.githubusercontent.com/40840760/152613759-75a00cce-fc46-4f5c-becb-656d1a869ebb.png)

<b> Below is a graph of relative rates of how much each complainant race files a complaint against WHITE police officers </b>

Findings:

1.	Native complainants have the highest rates of filing a complaint against a white police officer. 67% of officers reported by native complainants are white.
2.	White complainants are close in second place to file a complaint against white police officers.
3.	Black complainants have the lowest rates of filing complaints against white police officers. 47% of officers reported by black complainants are white officers.

![image](https://user-images.githubusercontent.com/40840760/152613814-f61e0346-d8cd-4177-a0f3-80a383a2f09f.png)

<b> Below is a graph of relative rates of how much each complainant race files a complaint against NATIVE police officers. </b>

There are only a few data points pertaining to native police officers, and they only make up a small percentage of police officers in the dataset. Hence, it is difficult to make any conclusions on very little data. Nonetheless, the data for filing rate against Native officers for each complainant race is as follows:

Unknown – 0.85%

Hispanic – 0.45%

White – 0.41%

Blacks – 0.32%

Native – 0%

Asian – 0%

For example, 0.45% of officers reported by Hispanics are Native.

For example, 0.41% of officers reported by Whites are Native.

![image](https://user-images.githubusercontent.com/40840760/152614524-86a0eed0-0074-497f-b317-c7c5f45b190f.png)


------------------------------------------------------------------------------
<p align=center> <font size="8"> <b> GENERAL FACTS: </b> </font> </p>

      1. Approximately 94% of complaints involve 3 or less police officers
      2. 66% of complaints only involve 1 police officer.
      3. 22% of complaints involve 2 police officers.
      4. 11569 complaints inolve only 1 police officer.
      5. 3867 complaints involve 2 police officers.
      6. 1034 complaints involve 3 police officers.

![image](https://user-images.githubusercontent.com/40840760/149868844-d0ed4c87-1a15-4b6c-9b38-f0ee9008f601.png)
      

