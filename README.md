# Analysis of Covid-19 and Vaccination Count Over the Past 30 Days

Team 1: Ranjani Anjur Venkatraman, Cody Gardner, Sharon Colson

## Overview: 
  The Covid-19 pandemic caused the shut down of many businesses and countries across the world in 2020. Now we have vaccine options available, and some portion of the population is utilizing them. As the number of vaccinated people rises, what is happening to the number of Covid-19 cases? As time passes are the numbers of new Covid-19 cases increasing, decreasing, or remaining static?
	These are questions that a business owner or manager may need answered to make an action plan for his company’s future. 

## 📊 Data & Models:
  To examine these questions, data was pulled, cleaned, and examined from the following sources:

•	API 1: https://disease.sh/v3/covid-19/historical -- to retrieve data over 30 days for cases, deaths, and recovered of Covid-19 across 181 countries.

•	API 2: https://disease.sh/v3/covid-19/vaccine/coverage/countries?lastdays=1 -- to retrieve vaccination data.

•	API 3: https://disease.sh/v3/covid-19/countries/ -- to retrieve present day Covid-19 information 

  It was merged and reorganized into many different DataFrames for further evaluation but the below are small portions of the two most utilized examples:


> #### For the evaluation of the change over time:
>  
> <div style="text-align: center;">
> <img src="https://user-images.githubusercontent.com/83737584/127934978-471a07bc-8367-4558-aa5d-72ec38f6c98f.png">
> </div>

<br>

> #### For a broader view of the effects of different variables:
>  
>
><div style="text-align: center;">
> <img src="https://user-images.githubusercontent.com/83737584/127934994-bab5ff26-d48f-4624-9cdc-919dce21a1e8.png">
</div>

<br>

  Once the data was collected, it was evaluated in different forms to verify trends. For example:

<br>

> ####   The Number of Vaccinated Versus Unvaccinated:
>
>![image](https://user-images.githubusercontent.com/83737584/127935021-e525db1c-a94e-4de0-a0e4-b6ac3c1bbd84.png)

 <br>

 > #### The Number of Cases and Recovered:
 >
 >![image](https://user-images.githubusercontent.com/83737584/127935053-249128d6-16a7-489a-85fa-b395f530a5a4.png)

  <br>

> ####  An Overall Evaluation of Cases, Deaths, and Recovered:
> 
> ![image](https://user-images.githubusercontent.com/83737584/127935082-3cfb242d-b2dd-46dc-a57b-9b8cc546fe21.png)
 
 <br>

 > ####  The Current Count of Deaths (Cross Section of the Most Affected Countries):
 >
 >![image](https://user-images.githubusercontent.com/83737584/127935106-06752c4d-7ad6-409c-8c3e-cceae8e24dc2.png)

<br>

> #### The Change In Cases Over the Last 30 Days:
> 
> ![image](https://user-images.githubusercontent.com/83737584/127935118-4988c670-ab64-4af9-8c7e-05f01abf022c.png)

<br>

## 📈 Results:
  In an effort to answer the original questions, the following hypothesis were established:

<br>

Hypothesis Set 1:

•	H0: Cases and Vaccination are independent

•	H1: There is a dependency between Cases and Vaccination

<br>

Hypothesis Set 2:

•	H0: a unit root is present (series is non-stationary).

•	 H1: a unit root is not present (series is stationary).¶

<br>

 > #### Through Linear Regression Analysis, a positive correlation between cases and vaccination count was determined with a P-value of 4.65x10-6. 
>
> ![image](https://user-images.githubusercontent.com/83737584/127935141-f812f53f-08cb-45cc-9823-b613952565c5.png)
>
>  This correlation was further quantified through calculation of the Pearson’s Correlation Coefficient at 0.33 with the same p-value. 

<br>

>  Additionally, using the Augmented Dickey Fuller test the second hypothesis set was evaluated with a p-value of 1.00 which tells us that data is not stationary. It was determined that as time advances, the number of new daily cases of Covid-19 increases. 
>
>![image](https://user-images.githubusercontent.com/83737584/127935165-a4037d59-a16d-4d18-b229-b158c2b8fa1b.png)

<br>

## 💡 Conclusion:
   Using the above mentioned analysis and calculations it has been determined that of Hypothesis Set 1, the alternative hypothesis, that there is a dependency between cases and vaccinations, appears to have been established; also, of Hypothesis Set 2, the null hypothesis, that there is a unit root present and the series is non-stationary. In other words, analysis of the data available indicates that while vaccination counts are rising, new Covid-19 cases are rising as well and as time advances they rise at a greater rate. 
	
   Further analysis based on a larger time frame (say 90 or 180 days) might give additional information. It could be that vaccination counts have not yet come to a number that would cause Covid-19 cases to fall or that the new Delta (or any subsequent) variant will cause Covid-19 cases to continue to rise despite increasing vaccination counts. At this time however, the suggestion of this analysis to any business owner or manager would be to prepare an action plan for further restrictions due to rise in Covid-19 cases. 
   
   <hr>
   
   Contact:

* https://www.linkedin.com/in/sharon-colson
* sharon.colson@gmail.com
	

