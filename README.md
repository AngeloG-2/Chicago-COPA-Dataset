<b> NOTE: A summary of insights found in the dataset is available below. </b>

# Chicago-COPA-Dataset

The Dataset used in this project can be found at: https://www.kaggle.com/chicago/chicago-copa-cases/version/20

# Quick Description of Dataset

1. Each row is a complaint by a person(s) submitted to an internal review board with an allegation that a police officer mistreated them in some way. 
2. Police complaints has two parties. The complainants and police officers. 
3. The data is from the Chicago Police Department

# Purpose of Project

The goal of the project is to perform a comprehensive deep-dive analysis of the following:

1. Analyze the races of complainants who filed different mistreatment allegations.
2. Analyze the races of police officers who allegedly mistreated civilians.
3. Determine if a particular race of complainants is more likely to file a complaint against a specific race of police officers.
4. Time-series analysis of the frequency of each mistreatment allegation.

# Files Description

NOTE: This project is a work in progress.

This project consists of four files.

1. Chicago COPA - Data Cleaning.ipynb -> This notebook focuses on cleaning and transforming raw data into more useful forms. Unfortunately, some columns in this dataset are extremely dirty and I had to perform extensive data cleaning.

2. Chicago COPA - Analysis.ipynb -> This notebook performs an extensive analysis of the races of police officers and complainants.

3. no_bia_with_officer_information.csv -> Cleaned dataset with all nesscessary columns.

4. copa-cases-summary.csv -> Original Dataset.

# Summary of Findings

<p align=center> <font size="8"> <b> Analysis of Races of Complainants Involved In Mistreatment Allegations </b> </font> </p>

This section analyzes the race distribution of complainants involved in police mistreatment allegations.

First, let us look at the race distribution of complainants from mistreatment allegations between 2008 to 2018. About 71% of complainants are black. While Hispanics make up 14.4% of complainants, Whites make up 10.4% of complainants. The other 4.2% are of other or unknown races.


![image](https://user-images.githubusercontent.com/40840760/156479211-42aa99b5-da83-4a99-b17e-980b91a4db8d.png)

As you can see above, blacks are disproportionately represented as complainants. Is it possible that Chicago is primarily black? This would explain the results. However, this is not the case. In 2016, 29.3% of people living in Chicago were black, yet blacks make up 70.5% of all complainants in mistreatment allegations.

Now the question is: have blacks always made up the majority of complainants? To analyze this, I created a graph below.

The graph below shows the relative frequency of each complainant's race between 2008 and 2018. The chart is interpreted like this: in 2010, approximately 18% of complainants were Hispanic.

![image](https://user-images.githubusercontent.com/40840760/156479304-84c4af6b-d5cb-42af-8e87-29eb683b226f.png)

From 2008 to 2018, blacks make up the majority of complainants by a substantial margin. In 2011, the relative frequency of black complainants was at its peak when 73.9% of complainants were black.

Moving on to analyzing the relative frequency of Native, Asian, Hispanic, and Whites. I created the graph below, similar to the graph above, except Blacks are excluded in the chart.

![image](https://user-images.githubusercontent.com/40840760/156479374-23c8d428-8afd-4dae-801c-a6bff68c750d.png)

Interestingly, the percentage of complainants that are Natives, Asians, Hispanics, and Whites has remained stable over 10 years. However, a larger percentage of complainants have Unknown races. The percentage contribution of complainants of Unknown races has increased from 1.03% in 2011 to 6.19% in 2018.

So far, I have analyzed the race distribution of complainants in two ways, on a year-by-year basis and an aggregate level from 2008 to 2018. My analysis did not take into account the type of mistreatment allegation. There are 20 types of mistreatment allegations in the dataset. A list of mistreatment allegations is provided by the image below.

![image](https://user-images.githubusercontent.com/40840760/156479412-06dac887-e69c-496c-982b-4ba576160c88.png)

Now, I will analyze the race distribution of complainants on a year-by-year basis grouped by the mistreatment allegation.

I will first analyze Excessive Force allegations. This is the most common type of allegation.

![image](https://user-images.githubusercontent.com/40840760/156479452-9da45882-e05d-4a5d-8f1b-8e4875b7cf67.png)

For Excessive Force complaints, blacks make up the largest percentage of complainants by a considerable margin, with an average percentage of 70.9% between 2008 and 2018.

![image](https://user-images.githubusercontent.com/40840760/156479478-30f30456-d146-4a81-84ed-972d5e48ffdc.png)

Looking more closely into the trend for black complainants. There was a massive spike in the relative frequency of black complainants for excessive force complaints. The percentage in 2017 was 66%, and in 2018, the percentage was 75%, the highest percentage value between 2008 to 2018.

Now, I will analyze the relative frequency of other races involved in excessive force complaints.

![image](https://user-images.githubusercontent.com/40840760/156479506-7d78acc4-737e-447e-b798-b8f504237c3b.png)

We can see that the most frequent excessive force complainants are in the following order: Blacks, Hispanics, Whites, Unknown, Asians, and Natives. The % complainants that are non-black have remained stable from 2008 to 2017. However, in 2018, there was a massive shift in the percentage frequency for all non-black complainant races. For example, the percentage of Whites complainants has decreased from 13% to 6.43%. Similarly, the percentage of complainants of Unknown races has increased from 2.64% to 5.6%.

Moving on to another type of mistreatment allegation. I will analyze the relative frequency of complainants who specifically filed for Taser Nonfiction complaints. Taser Notifications are the second most frequent complaint.

![image](https://user-images.githubusercontent.com/40840760/159610680-6c65eb01-88ad-4f9d-a9b3-3ba29ff4e29a.png)

The story is similar for Taser Notification complaints; Blacks make up the majority of complainants by a substantial margin. In fact, the margin of difference is slightly larger than Excessive Force complaints. At its peak, 78.57% of complainants in Taser Notification were black compared to 70.5% in excessive force complaints.

![image](https://user-images.githubusercontent.com/40840760/159610738-5c06c1bd-fab1-46dd-aa87-c4cf5467d3ce.png)

Looking more closely into the trends for black complainants who filed for taser notification complaints. We see a large spike in the relative frequency of Black complainants in 2009. From 67.51% in 2008, to 78.57% in 2009. From 2010 onwards, the relative frequency has remained stable for Black complainants. However, in 2018, relative frequency dipped from 77.2% to 71.42%, indicating that a lower percentage of complainants are black.

Moving on to analyzing the relative frequency of non-black complainants that filed for Taser Notification. 

![image](https://user-images.githubusercontent.com/40840760/159610883-3f6ccaae-ec9f-4f7f-9cfd-100fe0c71d73.png)

For non-black races, we see that Hispanics are the second most-frequent race who filed taser notifications, except in 2013, where Whites passed Hispanics. Whites are the third most frequent, followed by Unknown races, Asians, then Natives. Interestingly, rankings remained unchanged for Taser Notification over 10 years, which is similar to Excessive Force complainants. In addition, the percentage of complainants that are White who filed for Taser Notifications complaints had a sharp increase in 2018, from 6.8% to 14.28%.

Now, moving to another type of mistreatment allegation. I will analyze the relative frequency of complainants who specifically filed for Verbal Abuse complaints.

![image](https://user-images.githubusercontent.com/40840760/159611096-9c0c5269-ecce-4991-bd95-1ad938622123.png)

The story is similar for Verbal Abuse complaints; blacks make up the largest percentage of complainants by a substantial margin. However, there was a sharp decrease in % black complainants in 2018, from 77.35% to 52.77%.

Looking closer at the trends for Black complainants who filed Verbal Abuse complaints.

![image](https://user-images.githubusercontent.com/40840760/159611165-eb5aeb17-6aa2-4f03-9c44-934fc7346989.png)

The relative frequency for black complainants who filed for Verbal Abuse has been volatile between 2008 and 2017. With a minimum value of 67% to a maximum of 80%. We a sharp decrease in the % black complainants in 2018.

Now I will look at the trends for non-black complainants who filed for Verbal Abuse complaints.

![image](https://user-images.githubusercontent.com/40840760/159611210-d7520fbb-aa5e-4fde-b298-953fda50a6ae.png)

We can see that % of non-black complainants who filed for Verbal Abuse complaints have been very volatile, in fact, more volatile than Excessive Force or Taser Notification complaints. Regarding rankings, % Hispanics and % Whites have traded places for 2nd and 3rd places between 2008 and 2018. Meanwhile, % of complainants of Unknown races has steadily increased in from 2012 to 2018, suggesting reporting problems in the COPA organization. Lastly, % Asians complainants have remained relatively stable and are at 5th place.

So far, I have analyzed % complainants for 3 types of mistreatment allegations: Excessive Force, Taser Notification, and Verbal Abuse. We are noticing a consistent pattern; blacks make up the largest percentage of complainants by a substantial margin. But is this true for all types of mistreatment allegations? Let’s look at some data below.

![image](https://user-images.githubusercontent.com/40840760/159611261-174dd99a-32bd-4f51-a11c-9f569a2fadb3.png)
![image](https://user-images.githubusercontent.com/40840760/159611276-9150d21c-8465-4943-868a-f64c18a4c072.png)

The chart above has two columns named “black_complainant_rank” and “blackPercentage_secondHighest_difference (percentage).” The former is the ranking of black complainants in terms of % complainant. The latter is the margin difference between % black and the second-highest % complainant.

Out of 19 of 20 mistreatment allegations, Black complainants rank number one in terms of % complainants. What is more shocking is the margin of difference between % black complainants, and the second-highest % complainants range from 0% to 82.4%, with a median of 56.1%. This large margin of difference means that blacks have a substantial lead over the second-highest % complainant in almost every mistreatment allegation type.

The only mistreatment allegation where black complainants do not lead in % complainants is Legal Violations. In this case, Blacks are tied with another race.

So, what can we conclude in this analysis? I only analyzed black complainants in detail, so I can only make conclusions on black complainants. Let’s first recap our findings.

      1. Blacks make up 71.3% of complainants if we combine all mistreatment allegations from 2008 to 2018.
      2. From 2008 and 2018, blacks were the number one complainant in each year and had a massive lead of approximately 50%.
      3.Blacks complainants make up the majority of complainants by a substantial margin in 18 out of 20 mistreatment allegations—the median margin of difference is           56.1%.
 
My conclusion is that there are two possible reasons blacks are disproportionately represented as complainants. First, Black civilians in Chicago do not trust local police officers, and second, Blacks are being intentionally being targeted by the local police department. Which of these are true? It is hard to say because I don’t have information on what is happening on the ground. 

But we do have convincing evidence that Chicago has a potential problem with how its police officers treat Blacks; as a result, further investigation is necessary to determine what is actually happening.

------------------------------------------------------------

<p align=center> <font size="8"> <b> Analyzing the Races of Complainants and Police Officers   </b> </font> </p>
 
A complaint has two sides, complainants, who believe they were mistreated in some way by police officers, and the police officers themselves.

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
<p align=center> <font size="8"> <b> CORRELATION STUDY: </b> </font> </p>

Police complaints have two parties: the complainants and police officers. The correlation study aims to analyze correlations between the number of complainants and police officers involved in complaints. Below are the findings from the correlation analysis.

      1. The more black complainants are involved, the greater number of black police officers are involved.
      2. The more Hispanic complainants are involved, the greater number of Hispanic police officers are involved.
      3. The more white complainants are involved, the greater number of white police officers are involved.
      4. The more Hispanic complainants are involved, the lesser number of black police officers get involved.
      5. The more white complainants are involved, the lesser number of black police officers get involved.

      All five have a weak correlation but are statistically significant 
      due to extremely small p-values. 

![image](https://user-images.githubusercontent.com/40840760/158307213-195b1c66-4b67-4590-af04-7f91c1c52508.png)



------------------------------------------------------------------------------
<p align=center> <font size="8"> <b> GENERAL FACTS: </b> </font> </p>

      1. Approximately 94% of complaints involve 3 or less police officers
      2. 66% of complaints only involve 1 police officer.
      3. 22% of complaints involve 2 police officers.
      4. 11569 complaints inolve only 1 police officer.
      5. 3867 complaints involve 2 police officers.
      6. 1034 complaints involve 3 police officers.

![image](https://user-images.githubusercontent.com/40840760/149868844-d0ed4c87-1a15-4b6c-9b38-f0ee9008f601.png)
      

