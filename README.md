# Project_1
Covid-19 is a disease that has caused millions of deaths worldwide. Many people have lost their loved ones and their jobs because of it. The impact of this virus goes beyond health – it affects our economies and the environment. In this study, we focus on three distinct research questions, each aiming to shed light on the interactions between COVID-19 deaths and different factors.

## Question One: Does the number of COVID-19 deaths depend on GDP and income?

In the first question, we investigate the potential influence of economic indicators on COVID-19 mortality. Gross Domestic Product (GDP) is a widely recognized measure of a state's economic health, while per capita personal income reflects the income distribution among the population. Understanding the connection between these economic factors and COVID-19 deaths is crucial in assessing the pandemic's social and economic implications. To answer this question, we employ linear regression analysis with interaction effects to uncover the relationship between COVID-19 deaths and GDP and income in Texas during the year 2021.

## Question Two: Do states with warmer environments have a higher number of COVID-19 deaths?

The second question delves into the environmental factors affecting COVID-19 deaths. Specifically, we aim to determine whether states with warmer climates experience a higher number of COVID-19 fatalities in the year 2021. The motivation behind this question lies in the potential impact of temperature and humidity on the transmission and survival of the virus. We plan to employ U-test analysis to compare COVID-19 deaths between Texas, a state with a relatively warm climate, and Michigan, a state with colder weather, in order to assess the relationship between climate and COVID-19 mortality.

## Question Three: Do higher unemployment rates in 2021 in Florida compared to Alabama result in higher COVID-19 deaths?

The third question revolves around the interplay between employment rates and COVID-19 mortality. The economic consequences of the pandemic, including job losses, have been substantial. To gain a deeper understanding of this aspect, we will investigate whether higher unemployment levels in Florida compared to Alabama in 2021 resulted in a greater number of COVID-19 deaths. This analysis helps us assess the social and health impacts of economic disparities during the pandemic. We plan to use U-test analysis to compare COVID-19 deaths between the two states, shedding light on the potential correlation between unemployment and COVID-19 mortality.

# Results 

## Question One: Does the number of COVID-19 deaths depend on GDP and income?

After fitting the data for 

## Question Two: Do states with warmer environments have a higher number of COVID-19 deaths?

In this analysis, I aimed to investigate whether states with warmer climates, represented by Texas, have a higher number of COVID-19 deaths compared to a state with colder weather, such as Michigan, in the year 2021. I have collected COVID-19 death data and I noticed that both data are not normally distributed as shown below :

<p align="center">
<img src="https://github.com/baa151/Project_1/assets/123330888/11f07067-8772-4881-b3bc-3c4d090af7a1" width="400" height="300" alt="Image 1">
<img src="https://github.com/baa151/Project_1/assets/123330888/18f65745-d47b-40e7-ba38-e62ed3139dea" width="400" height="300" alt="Image 2">
</p>


Thus, I have conducted a Mann-Whitney U test, which can be used when the data do not follow a normal distribution, with a null hypothesis ($H_0$) that says there is no significant difference in COVID-19 deaths between Texas and Michigan, and an alternative hypothesis ($H_a$) that there is a significant difference.

<p align="center">
<img src="https://github.com/baa151/Project_1/assets/123330888/aef1f970-d86e-4e65-b1d5-feae7cb22a47" width="600" height="400" alt="Image 3">
</p>

where: 
U statistic: 8999.0
P-value    : 0.0508
Fail to reject the null hypothesis: There is no significant difference in COVID-19 deaths between Texas and Michigan.

The results above suggest that : For the specific states of Texas and Michigan in 2021, the climate difference does not seem to have a significant impact on the number of COVID-19 deaths. This may indicate that other factors, such as vaccination rates and population density, play a more prominent role in determining COVID-19 mortality.
Note : It's important to note that while this analysis focuses on two states, the implications may not be generalized to all states. Different states may experience varying impacts of climate on COVID-19.

## Question Three: Do higher unemployment rates in 2021 in Florida compared to Alabama result in higher COVID-19 deaths?

In this analysis, I aimed to investigate whether higher unemployment rates in Florida compared to Alabama in 2021 resulted in a greater number of COVID-19 deaths. I have collected COVID-19 death data and I noticed that both data are not normally distributed as shown below :

<img src="https://github.com/baa151/Project_1/assets/123330888/9a2315a4-97db-40fa-a4b8-a34a28627ddc" width="400" height="300" alt="Image 4">
<img src="https://github.com/baa151/Project_1/assets/123330888/442e8c24-2baa-494b-90bf-014334c6f2f2" width="400" height="300" alt="Image 5">

Thus, I have conducted a Mann-Whitney U test again, with a null hypothesis ($H_0$) that says there is no significant difference in COVID-19 deaths between Alabama and Florida in 2021, and an alternative hypothesis ($H_a$) that there is a significant difference.

<p align="center">
<img src="https://github.com/baa151/Project_1/assets/123330888/5c8ba785-1706-4b08-93e0-deb5299c2bd7" width="600" height="400" alt="Image 6">
</p>

where:
U statistic: 1700.0
P-value: 0.0155
Reject the null hypothesis: There is a significant difference in COVID-19 deaths between Alabama and Florida.

The results above suggest that : There is a meaningful relationship between unemployment rates and COVID-19 deaths, with Florida experiencing higher mortality compared to Alabama. Higher unemployment levels in Florida appear to be associated with a greater number of COVID-19 deaths during the year 2021. The findings imply that economic disparities, particularly those related to unemployment, can have health consequences during a pandemic. Understanding this relationship is important for public health and policy decisions, as targeted interventions and support measures may be needed in areas with higher unemployment rates.
This underscores the importance of considering the social and economic aspects when assessing the impact of the pandemic
