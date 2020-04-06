### Using Small Area Estimation and Machine Learning for Improved Poverty Assessments throughout Ethiopia and Eastern Africa 
<p align="center">
  <b>by Larry Feng</b><br>
  <b>April 5, 2020</b><br>
  <b>2664 words</b><br>
</p>

### Introduction

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The objective of this research is to improve upon the use of Small Area Estimation and machine learning methods to generate more accurate maps and reductions of poverty rates across mainly Ethiopia and other countries in Eastern Africa by validating different statistical models as compares to using previous census data to estimate these models. On the topic of census data: even for a developed, superpower country such as North America, we can only take a census of the whole population every 10 years. Although census data is of the most accurate data one can get, they just are not efficient. Further, the ability of census data continues to decline each year after a census is taken, due to the dynamic nature of the world. It is hard for static data to accurately describe a population that is ever changing; each hour results in movement and shifts. Through the combination of Small Area Estimation, survey data, and machine learning methods, more accurate models are produced to describe and predict poverty, with results of higher quality than traditional statistical methods while using less time and less resources. Central to achieving this research goal of improving the usage of Small Area Estimation and machine learning methods, the model for predicting and mapping poverty will be increasing the resolution of the location of the population and maps of population from low resolution to high resolution models. I will achieve this goal through meeting the following objective.

1. Use data provided by the governments of Ethiopia and Eastern Africa to estimate the levels of poverty and poverty reduction rates. 

2. Use survey data collected from Small Area Estimation to estimate a machine learning model for predicting the poverty levels of all populations across Africa.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This work will build on previous research by Mezemir Wagaw, Tommy L. Coleman, Teferi D. Tsegaye, Wubishet Tadesse, Xinsehn Diao, Alejandro N. Pratt, Emily Schmidt, Mekamu Kedir, Atreshiwal Girma, Christine Husmann, Thomas P. Sohnesen, Niels Stender, The World Bank, Arne Bigsten, Bereket Kebede, Abebe Shimeles, Mekonnen Taddesse, Valerie Graw, Christine Ladenburger, Caitlin Brown, Martin Ravallion, Dominique van de Walle, and their respective teams, and will incorporate new methods to implement an understanding of poverty as well as recent advances towards inferring poverty mapping, prediction, and estimation.[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

### Human Development Topic 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Poverty has been an ongoing issue in the world for as long as anyone can remember. As the world and countries develop, the poverty line has been driven down; however, the poverty rate can never be driven down to zero percent. In addition, poverty is especially prevalent in Ethiopia with numbers around seventy to eighty percent of the population living in some type of poverty. With the majority of the population affected by some sort of poverty, I can conclude that millions of people are suffering, not from inconveniences, but from factors that prevent them from thriving. As the citizens continue living in poverty, many issues arise, such as: inadequate access to health care, tight living spaces, unclean household areas, food security, susceptibility to disease, and below average household incomes. The inherency of poverty can come from a plethora of factors, but some of the ones discussed seem to focus on agriculture. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Amartya Sen, Professor of Economics and Philosophy at Harvard University, revolutionized the meaning of “human development”. According to Sen, “human development is a process of enlarging people’s choices of which freedom increases the citizen’s access and opportunities to the things that have reason to value”. Does poverty count as a unfreedom? Well, first we have to earn an understanding of exactly what poverty is. As mentioned in the introduction of *Remote Sensing and GIS Based Poverty Mapping Small- Area Estimation Approach*, “there is no agreed international definition of poverty”. Girma states that poverty can take on many forms that one might not even realize, such as: hunger, lack of shelter, being sick and not having access to doctor, no access to school, illiteracy, not having a job, fear of what’s to come in the future, living each day as a struggle. [1] Poverty is powerlessness, a lack of representation and freedom. By the definition of government, poverty is whether one’s consumption or income level falls below the minimum level necessary to meet basic needs, called the “poverty line”. Each country, however, has different basic needs and different minimum income levels, so these poverty lines vary in time and place. Throughout the whole world, the universal definition of poverty is the lack of basic necessities required to survive- this includes food, water, and shelter. However, it is unacceptable to think of the universal definition as the main definition. If poverty means the minimum to survive, then this issue is one of the biggest unfreedoms regarding human development. In general, however, no matter the type discussed, poverty is an unfreedom by the definition of human development according to Sen. Poverty is the opposite of increasing citizen’s access and opportunities to the things they have reason to value. Poverty restricts the freedom of a person’s actions, since they have to set that money to afford the basic needs for humans. Poverty confines a person’s choices, unable to see a doctor even if they have a life-threatening disease. Poverty is an unfreedom that affects million of people around the world. There are currently relief aid plans in place to help countries that are afflicted by this problem. There is a chance, however, that the aid ends up in the wrong hands. It does not matter if the aid arrives in the country. Only until the aid reaches every household it intends to, will the job be complete. But, if the country providing aid does not know where to send help, poverty continues to increase. So, with the aid of Small Area Estimation and machine learnings techniques, the data collected from these countries can be transformed into high-resolution maps that reveals the location of where the poverty reside.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;There are a couple sustainable development goals that relate to this human development topic, but there is one that is significantly more applicable than the others: No poverty. As for the other goals, I disagree with how many sustainable development goals (SDG) there are. The United Nations Member States lists many goals that can be defined under poverty such as: hunger, health, education, clean water, inequalities, employment. Under the United Nations Member States full report, though, they do list many factors that can be defined under poverty. They state, “Poverty is a multi-dimensional phenomenon”. But, relating back to SDG’s, I think this reveals the significance of poverty. Listed as number one, poverty is the first issue that the sustainable developments goals address. And, according to Sen, removing unfreedoms is the path to becoming a fully developed country. [1]

### Human Development Process

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Poverty is a key concern in many countries. According to Husmann, of the eighty-six million people living in Ethiopia, around eighty percent living in rural areas are in severe poverty. In addition, the official poverty headcount in 2011 is 26.9%. [2] Over the span of 10 years, there has been an undefined trend in reducing poverty. In 1995 to 2005, rural poverty rates dropped from 48 to 39 percent while urban poverty rates have increased from 33 to 35 percent over the same time period. [3] It seems, compared to the other sources, rural poverty rates continue to drop, while urban poverty rate increase. We will look further into the roots of poverty: the institutions, social services, infrastructures, land use, urban/suburban contexts, accessibility to infrastructures, and whether poverty behaves as a complex adaptive social/economic system. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Limiting poverty to a simple definition of income, resources, or service deficit does not accurately describe the complex, emergent nature of poverty. But, it may be more helpful to view the social ecology that inherently generates poverty as a type of complex adaptive system. By doing this, we acknowledge the many components interacting within each other, the social, cultural, and economic components that are individually and all-together adapting. This type of ‘mental’ model benefits our understanding of the role of different drivers and agents, collectively and individually, and it also reveals a holistic and more integrated set of strategies that are designed to influence factors at varying levels. Furthermore, it leads to strategies less focused on the construction of isolated interventions and more on how the poverty system itself functions, along with factors that impact the system’s resilience and capability to respond directly. [11]

### Geospatial Data Science Methods

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The data science methods I will be looking at are Small Area Estimation and Random Forest technique. First, Small Area Estimation (SAE) has been gaining popularity among development practitioners worldwide. [9] In the SAE method, consumption levels are imputed for each household in the population census based on a consumption model estimated from a survey. The consumption model must include explanatory variables, household and individual. Applying the estimated coefficients to these same variables in the census data, the consumption expenditures can be credited to each household. Then, poverty for small areas can be predicted based on this accredited per capita consumption. One of the advantages of SAE is that it not only estimates “poverty incidence”, but it also produces predictions of standard errors on the estimates. Because the poverty estimates are produced based on the imputed consumption, there will definitely be “imputation errors”, and they will be revealed in the standard error. SAE has two stages: first, we use an equation with the log per capita consumption expenditures, *ln y<sub>ch</sub>*,

<p align="center">
  <i>ln y<sub>ch</sub> = X'<sub>ch</sub>β + Z'γ + u<sub>ch</sub></i>
</p>

where X'<sub>ch</sub> is the vector of explanatory variables for household *h* in the cluster *c*. β is the vector of associated regression coefficients, Z' is the vector of location specific variables with γ as the associated vector of coefficients, and *u<sub>ch</sub>* is the regression disturbances due to the discrepancy between the predicted household consumption and the actual value. The estimates from SAE can be validated by comparing the numbers estimated with the data itself. In this case, the data is retrieved from the Bhutan Living Standard Survey. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/58920498/78520384-5ef1ee00-7794-11ea-9a7b-c65f226c64f5.png">
</p>
<p align="center">
  [9] <i>The World Bank</i>. (2010, June). Small Area Estimation of Poverty in Rural Bhutan.
</p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The ‘key’ variables in the graph correspond to the BLSS data, representative of the district level. Presumably, if the underlying assumption that homogeneity and stability from 2005 to 2007 do not hold, there is little reason to anticipate estimates from the SAE method to be similar to the data itself. Conversely, if the SAE method produces a superb predictor of “true poverty incidence”, it would be relatively similar to the BLSS data.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Second, the Random Forest (RF) model which stems from machine learning algorithms. RF often produces higher accuracy poverty predictions, particularly at the urban and rural levels, as compared to the national level. But, RF is an automated tool, one that requires a low level of knowledge to operate, and it performs just as well or even better than classical statistical methods. The RF method is exactly what the name is: a multitude of trees that can be called a forest. It consists of decision trees, and each tree contains a number of decision nodes. Inside each node, data is split according to how well the variable can predict poverty. To keep it simple, RF can be split into a few steps:

1. Split the data in half, leaning and evaluation sample
2. Draw a random sample of two-thirds the observations with replacement for each tree from the ‘learning’ data set
3. Grow a tree:
   * For every node in the tree, take a random sample of √n, where n is the total number of variables.
   * Select the variable used for splitting in each node with the lowest entropy (disturbance)
   * Grow each tree until a split leads to fewer than 4 observations in each leaf
4. Repeat steps 2 and 3 a few hundred times. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Based on the couple hundred of trees, the output is the “score function” that a household is calculated to be in poverty or not. So, each tree predicts the status for a household. According to *World Bank*, Random Forest is a good predictor of poverty, and sometimes it is better than current methods. It is not the most accurate method, but it is more robust and does not make large prediction errors. Overall, Random Forest is a simple, automated method to take advantage of and can be used as a complement to other methods. [10]

### Discussion 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;At this point in my research, I feel like I have a more complete understanding of the definition of poverty and how it relates to human development. In addition, each data science method by itself can be weak and produce dissatisfactory results. With a single method, the results can be clouded in errors and can not be used by other people to make accurate predictions on the subject. But with both methods complementing each other, they can fill up where the other falls short. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I believe that there will always be a gap in the research. It is just not possible for a research project to cover absolutely everything that could have an impact on poverty in the world. There are also cases in which factors that we think affect the issue do not actually impact it at all, but we do not possess any research or the means to produce the research to disprove it. But, I do think one gap in most researches on this subject is the lack of poverty mapping. Recent studies are highlighting the importance of geography and spatial data as determinants of poverty. Yet most of recent research is limited to elementary and one-dimensional characterizations of the roles of regions and access to different types of infrastructure, public services, and markets. Many poverty mapping exercises just simply rank areas by a level of poverty or marginality indicator and completely disregard the use for maps. [1] My research question produced from my analysis in this literature review is whether Small Area Estimation Technique and Random Forest Model is effective, cheaper, faster, and able to stay relevant compared to other current methods on poverty assessments in developing countries.  

### References

[1] Girma, A. (2012, June 1). Remote Sensing and GIS Based Poverty Mapping Small- Area Estimation Approach in Rural Oromiya Regional State. Retrieved February 13, 2020, from 
[http://etd.aau.edu.et/handle/123456789/5098](http://etd.aau.edu.et/handle/123456789/5098)

[2] Husmann, C. (2015, November 3). Marginality as a Root Cause of Poverty: Identifying Marginality Hotspots in Ethiopia. Retrieved February 13, 2020, from 
[https://www.sciencedirect.com/science/article/pii/S0305750X15002466](https://www.sciencedirect.com/science/article/pii/S0305750X15002466)

[3] Schmidt, E., & Kedir, M. (2009, October). Urbanization and Spatial Connectivity in Ethiopia: Urban Growth Analysis Using GIS. Retrieved February 13, 2020, from 
[http://ebrary.ifpri.org/utils/getfile/collection/p15738coll2/id/130941/filename/131152.pdf](http://ebrary.ifpri.org/utils/getfile/collection/p15738coll2/id/130941/filename/131152.pdf)

[4] Diao, X., & Pratt, A. N. (2006, July 13). Growth options and poverty reduction in Ethiopia – An economy-wide model analysis. Retrieved February 13, 2020, from 
[https://reader.elsevier.com/reader/sd/pii/S0306919206000716?token=69C3F3D358B3D796CBEAA298AF6085D12A8D1DBE13E421830CEC237FAF63B8612EF2634F84F0309C9ECBD7499EC38C3E](https://reader.elsevier.com/reader/sd/pii/S0306919206000716?token=69C3F3D358B3D796CBEAA298AF6085D12A8D1DBE13E421830CEC237FAF63B8612EF2634F84F0309C9ECBD7499EC38C3E)

[5] Wagaw, M., Coleman, T. L., Tsegaye, T. D., & Tadasse, W. (2005, April 23). GIS Implementation to Support Poverty Reduction Policy and Drought Management in Ethiopia. Retrieved February 13, 2020, from 

[http://repository.uneca.org/bitstream/handle/10855/3606/Bib-28799.pdf?sequence=1](http://repository.uneca.org/bitstream/handle/10855/3606/Bib-28799.pdf?sequence=1)

[6] Brown, C., & Ravallion, M., & Walle, D. (2016, December). A Poor Means Test? Econometric Targeting in Africa. Retrieved March 29, 2020, from

[https://www.nber.org/papers/w22919.pdf](https://www.nber.org/papers/w22919.pdf)

[7] Graw, V., & Ladenburger, C. (2012, January). Mapping Marginality Hotspots – Geographical Targeting for Poverty Reduction. Retrieved March 29, 2020, from

[https://www.zef.de/fileadmin/user_upload/wp88.pdf](https://www.zef.de/fileadmin/user_upload/wp88.pdf)

[8] Bigsten, A., & Kebede, B., & Shimeles, A., & Taddesse, M. (2003, January). Growth and Poverty Reduction in Ethiopia: Evidence from Household Panel Surveys. Retrieved March 28, 2020, from

[https://www.economics.handels.gu.se/digitalAssets/1378/1378647_ethiopia-wd-2002.pdf](https://www.economics.handels.gu.se/digitalAssets/1378/1378647_ethiopia-wd-2002.pdf)

[9] The World Bank. (2010, June). Small Area Estimation of Poverty in Rural Bhutan. Retrieved March 28, 2020, from

[https://openknowledge.worldbank.org/bitstream/handle/10986/12348/681790ESW0WHIT0erty0in0Rural0Bhutan.pdf?sequence=1&isAllowed=y](https://openknowledge.worldbank.org/bitstream/handle/10986/12348/681790ESW0WHIT0erty0in0Rural0Bhutan.pdf?sequence=1&isAllowed=y)

[10] Sohnesen, T., & Stender, N. (2016, March). Is Random Forest a Superior Methodology for Predicting Poverty? An Empirical Assessment. Retrieved March 28, 2020, from

[http://documents.shihang.org/curated/zh/777401467987858907/pdf/WPS7612.pdf](http://documents.shihang.org/curated/zh/777401467987858907/pdf/WPS7612.pdf)

[11] Halfon, N. (2016, April). Poverty, Complexity, and a New Way Forward. Retrieved March 29, 2020, from

[https://www.academicpedsjnl.net/article/S1876-2859(16)00034-6/fulltext](https://www.academicpedsjnl.net/article/S1876-2859(16)00034-6/fulltext)
