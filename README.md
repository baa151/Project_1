# Project_1
Covid-19 is a disease that has caused millions of deaths worldwide. Many people have lost their loved ones and their jobs because of it. In this study, I will focus on three distinct research questions, each aiming to shed light on the potential relationship between COVID-19 deaths and different factors.

## Question One: Does the number of COVID-19 deaths depend on GDP and income?

I investigate the potential influence of economic indicators on COVID-19 mortality. Gross Domestic Product (GDP) is a widely recognized measure of a state's economic health, while per capita personal income reflects the income distribution among the population. Understanding the connection between these economic factors and COVID-19 deaths is crucial in understanding the potential factors that may have an impact on deaths cased by deseases. To answer this question, a linear regression analysis with interaction effects is applied to uncover the relationship between COVID-19 deaths and GDP and income in Texas during the year 2021.

## Question Two: Do states with warmer environments have a higher number of COVID-19 deaths?

In this question I aim to understand whether enviromental factors affects the number of COVID-19 deaths. Specifically, I aim to determine whether states with warmer climates experience a higher number of COVID-19 fatalities in the year 2021. The motivation behind this question lies in the potential impact of temperature and humidity on the transmission and survival of the virus. A U-test analysis is applied to compare COVID-19 deaths between Texas, a state with a relatively warm climate, and Michigan, a state with colder weather, in order to assess the relationship between climate and COVID-19 mortality.

## Question Three: Do higher unemployment rates in 2021 in Florida compared to Alabama result in higher COVID-19 deaths?

In this question I aim to understand the interplay between unemployment rates and COVID-19 mortality. The motivation behind this question stems from previous research that has showed that unemployment rates can lead to higher mortality from other diseases such as cardiovascular diseases. To gain a deeper understanding of this aspect, I will investigate whether higher unemployment levels in Florida compared to Alabama in 2021 resulted in a greater number of COVID-19 deaths. This analysis helps us assess the social and health impacts of economic disparities during the pandemic. A U-test analysis is applied to compare COVID-19 deaths between the two states, shedding light on the potential correlation between unemployment and COVID-19 mortality.

# Results 

## Question One: Does the number of COVID-19 deaths depend on GDP and income?

In this analysis, I aimed to investigate whether the number of COVID-19 deaths in Texas in 2021 depends on economic factors, specifically Gross Domestic Product (GDP) and per capita personal income. I used a linear regression model with interaction effects to explore this relationship. The results are shown below with a linear regression equation of $y = a x_1 + b x_2 + c x_1 x_2 + d$ :


$x_1 :  GDP$

$x_2 : Income$

$x_1 x_2 : Interaction$

$d : Intercept$

<p align="center">
<img src="https://github.com/baa151/Project_1/assets/123330888/9c9d14c6-74d7-4cb5-97e7-6fdee58b9026" width="700" height="400" alt="Image 1">
</p>

Notes :

- Both GDP and the interaction term have p-values less than 0.05, indicating their statistical significance as predictors of COVID-19 deaths.

- Income, with a p-value of 0.489, is not statistically significant in this model.

- The constant term 33.31, represents the estimated number of COVID-19 deaths when GDP and income are both zero.

This shows that states with a stronger economic foundation may have more resources to allocate to healthcare infrastructure, testing, and public health interventions, which can contribute to lower mortality.The negative coefficient implies that as this interaction increases, COVID-19 deaths decrease, although the coefficient is small. This could mean that regions with a strong economy and a fair income distribution may experience better health outcomes during a pandemic. The non-significance of income as a predictor of COVID-19 deaths in this specific context could be attributed to several factors. It's possible that income alone may not be a strong predictor because it doesn't capture the comprehensive impact of economic conditions. Income distribution, while important, might not be as influential as the overall economic well-being of the state, as represented by GDP. 

So, 

## Question Two: Do states with warmer environments have a higher number of COVID-19 deaths?

In this analysis, I aimed to investigate whether states with warmer climates, represented by Texas, have a higher number of COVID-19 deaths compared to a state with colder weather, such as Michigan, in the year 2021. I have collected COVID-19 death data and I noticed that both data are not normally distributed as shown below :

<p align="center">
<img src="https://github.com/baa151/Project_1/assets/123330888/6b5a8f23-c2ec-4cea-ae0e-fde17215f4e8" width="400" height="300" alt="Image 1">
<img src="https://github.com/baa151/Project_1/assets/123330888/f64c31c8-63c1-4436-9363-7095f3b9bf17" width="400" height="300" alt="Image 2">
</p>


Thus, I have conducted a Mann-Whitney U test, which can be used when the data do not follow a normal distribution, with a null hypothesis ($H_0$) that says there is no significant difference in the mean number of COVID-19 deaths between Texas and Michigan, and an alternative hypothesis ($H_a$) that there is a significant difference.

<p align="center">
<img src="https://github.com/baa151/Project_1/assets/123330888/aef1f970-d86e-4e65-b1d5-feae7cb22a47" width="600" height="400" alt="Image 3">
</p>

where: 

P-value    : 0.004382

Mean number of deaths for Michigan = 347.18

Mean number of deaths for Texas = 295.34

Reject the null hypothesis: There is a significant difference in COVID-19 deaths between Texas and Michigan.

This suggests that regions with colder climates may experience a higher number of COVID-19 deaths. There are several factors that could contribute to this pattern.
Firstly, during colder seasons, individuals are often exposed to less sunlight, which can lead to lower levels of vitamin D production in the body. Vitamin D plays a crucial role in supporting the immune system, and its deficiency can weaken immune responses. Secondly, research has indicated that viruses, including the SARS-CoV-2 virus responsible for COVID-19, can spread more easily in certain weather conditions, such as windy conditions. Wind can disperse respiratory droplets containing the virus over longer distances, potentially increasing the risk of transmission in colder, windy climates.

## Question Three: Do higher unemployment rates in 2021 in Florida compared to Alabama result in higher COVID-19 deaths?

In this analysis, I aimed to investigate whether higher unemployment rates in Florida compared to Alabama in 2021 resulted in a greater number of COVID-19 deaths. I have collected COVID-19 deaths data and I noticed that both data are not normally distributed as shown below :

<p align="center">
<img src="https://github.com/baa151/Project_1/assets/123330888/02b2febb-469e-4e53-8d5b-b4a1fa853d8c" width="400" height="300" alt="Image 4">
<img src="https://github.com/baa151/Project_1/assets/123330888/25481e7f-9fbb-4713-b969-3e48a52c6080" width="400" height="300" alt="Image 5">
</p>


Thus, I have conducted a Mann-Whitney U test again, with a null hypothesis ($H_0$) that says there is no significant difference in the mean number COVID-19 deaths between Alabama and Florida in 2021, and an alternative hypothesis ($H_a$) that there is a significant difference.

<p align="center">
<img src="https://github.com/baa151/Project_1/assets/123330888/1f4a17c2-05f5-49aa-a1ea-f038e3366f27" width="600" height="400" alt="Image 6">
</p>

where:

P-value: 0.20076 

Fail to reject the null hypothesis: There is no significant difference in COVID-19 deaths between Alabama and Florida.

The analysis revealed that unemployment did not have a significant effect on COVID-19 deaths in the states of Texas and Michigan during the year 2021. However, it is important to note that these findings are specific to these two states and this particular time period. Further research is needed to assess the impact of unemployment on COVID-19 deaths in other states and to understand how this relationship may vary under different circumstances.
