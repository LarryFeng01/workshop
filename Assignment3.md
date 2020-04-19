### Data Techniques of Predicting Poverty Throughout Ethiopia and Eastern Africa 
<p align="center">
  <b>by Larry Feng</b><br>
  <b>April 19, 2020</b><br>
  <b>1884 words</b><br>
</p>

### Introduction

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Poverty has been an ongoing issue in the world for as long as anyone can remember. As the world and countries develop, the poverty line has been driven down; however, the poverty rate can never be driven down to zero percent. In addition, poverty is especially prevalent in Ethiopia with numbers around seventy to eighty percent of the population living in some type of poverty [2,3]. As the citizens continue living in poverty, many issues arise, such as: inadequate access to health care, tight living spaces, unclean household areas, food security, susceptibility to disease, and below average household incomes. The inherency of poverty can come from a plethora of factors, but some of the ones discussed seem to focus on agriculture. Most studies conclude that if agricultural methods were improved such that food shortages can be cut; the poverty rate could be driven down. But what is poverty? As mentioned by Girma, “there is no agreed international definition of poverty” [1]. The author states that poverty can take on many forms that one might not even realize, such as: hunger, lack of shelter, being sick and not having access to doctor, no access to school, illiteracy, not having a job, fear of what’s to come in the future, living each day as a struggle. Poverty is powerlessness, a lack of representation and freedom. By the definition of government, poverty is whether one’s consumption or income level falls below the minimum level necessary to meet basic needs, called the “poverty line”. Each country, however, has different basic needs and different minimum income levels, so these poverty lines vary in time and place. In general, poverty mapping information is a “means to any persuasive framework” [1]. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The geospatial data science techniques I have decided to focus on is Small Area Estimation and Random Forest Model. I will further explain these techniques later in more detail throughout the methodological investigation. My research question produced from my previous analysis is whether Small Area Estimation Technique and Random Forest Model is effective, cheaper, faster, and able to stay relevant compared to other current methods on poverty assessments in developing countries. Small Area Estimation Technique is a newer statistical model used to predict poverty in lower income countries. It is increasing its popularity since it is currently the most effective statistical model while keeping funds into account. Of course, there exist better, more accurate methods, but Small Area Estimation (SAE) is known for using census/survey data and trying to keep costs low. The other method is Random Forest Technique. Random Forest Technique (RF) is a machine learning method that doesn’t adhere to statistical methods. It evolves along with bigger data, becoming more accurate with larger amounts of data. RF technique can be used for predictions of long, disordered regions in protein sequences, classification of agricultural practices based on satellite imagery, spatially distributed measurements of environmental conditions, and segmentation of video objects [10]. It is noted in Sohnesen that RF is usually applied to areas of research relating to medical literature, but not really in economics literature. In addition, the method has a better ability to predict because of its handling with non-linearities; this method, however, does not seem to hold its own when dealing with linear variables. 

### Inquiry Type

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This research question is evaluative since it wishes to find the most effective technique/method for predicting poverty. The purpose is to research the two methods, find the advantages of each while also considering their disadvantages. In the end, the two methods will be compared to reveal which is better for a lower-middle income country to use. Additional questions for this inquiry are: how much does the accuracy fall when using outdated census data? How many countries can this research be applied to? How do governments affect the running of poverty assessments? 

### Methods

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;First, Small Area Estimation (SAE) has been gaining popularity among development practitioners worldwide [9]. SAE is known for taking its data from census data, which has plenty of flaws, mainly inaccuracy. There is not much of a point to conduct a poverty assessment of Ethiopia in 2020 using 2007 census data because we would be predicting the past. Below is a figure where Girma analyses data and chooses which source is the most effective.

<p align="center">
  <img src="https://user-images.githubusercontent.com/58920498/79700486-0296d000-8264-11ea-922a-8e06a08fea1b.png">
</p>
<p align="center">
  Figure 1: Flow chart to analyze attribute data
</p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the SAE method, consumption levels are imputed for each household in the population census based on a consumption model estimated from a survey. The consumption model must include explanatory variables, household and individual. Applying the estimated coefficients to these same variables in the census data, the consumption expenditures can be credited to each household. Then, poverty for small areas can be predicted based on this accredited per capita consumption. One of the advantages of SAE is that it not only estimates “poverty incidence”, but it also produces predictions of standard errors on the estimates. Because the poverty estimates are produced based on the imputed consumption, there will definitely be “imputation errors”, and they will be revealed in the standard error. SAE has two stages: first, we use an equation with the log per capita consumption expenditures, *ln y<sub>ch</sub>*,

<p align="center">
  <i>ln y<sub>ch</sub> = X'<sub>ch</sub>β + Z'γ + u<sub>ch</sub></i>
</p>

where X'<sub>ch</sub> is the vector of explanatory variables for household *h* in the cluster *c*. β is the vector of associated regression coefficients, Z' is the vector of location specific variables with γ as the associated vector of coefficients, and *u<sub>ch</sub>* is the regression disturbances due to the discrepancy between the predicted household consumption and the actual value. There are a couple of variations in regard to the statistical equation, but most researchers use a variation of the equation above with similar variables. The estimates from SAE can be validated by comparing the numbers estimated with the data itself. In this case, the data is retrieved from the Bhutan Living Standard Survey. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/58920498/78520384-5ef1ee00-7794-11ea-9a7b-c65f226c64f5.png">
</p>
<p align="center">
  Figure 2:<i>The World Bank</i>. (2010, June). Small Area Estimation of Poverty in Rural Bhutan.
</p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The ‘key’ variables in the graph correspond to the BLSS data, representative of the district level. Presumably, if the underlying assumption that homogeneity and stability from 2005 to 2007 do not hold, there is little reason to anticipate estimates from the SAE method to be similar to the data itself [9]. Conversely, if the SAE method produces a superb predictor of “true poverty incidence”, it would be relatively similar to the BLSS data. Other results, such as in Girma, use the results from the equation for poverty mapping. In the figure below, the findings are produced to the woreda level (districts in Ethiopia) because market accessibility needs this level of detail to correlate with other georeferenced data [1]. The eastern region shows high rates of poverty, and the western area shows low to medium rates of poverty.

<p align="center">
  <img src="https://user-images.githubusercontent.com/58920498/79700565-936dab80-8264-11ea-9448-7291c5470f6b.png">
</p>
<p align="center">
  Figure 3: Rural poverty mapping of Ethiopia (Oromiya regional state) to the woreda level
</p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Second, the Random Forest (RF) model which stems from machine learning algorithms. RF often produces higher accuracy poverty predictions, particularly at the urban and rural levels, as compared to the national level. But, RF is an automated tool, one that requires a low level of knowledge to operate, and it performs just as well or even better than classical statistical methods. The RF method is exactly what the name is: a multitude of trees that can be called a forest. It consists of decision trees, and each tree contains a number of decision nodes. Inside each node, data is split according to how well the variable can predict poverty. To keep it simple, RF can be split into a few steps:

1. Split the data in half, leaning and evaluation sample
2. Draw a random sample of two-thirds the observations with replacement for each tree from the ‘learning’ data set
3. Grow a tree:
   * For every node in the tree, take a random sample of √n, where n is the total number of variables.
   * Select the variable used for splitting in each node with the lowest entropy (disturbance)
   * Grow each tree until a split leads to fewer than 4 observations in each leaf
4. Repeat steps 2 and 3 a few hundred times. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/58920498/79700595-c4e67700-8264-11ea-9d07-832684d482de.png">
</p>
<p align="center">
  Figure 4: Example of classification tree with three predictors(X<sub>1...X<sub>3) with two classes and five partitions(R<sub>1…R<sub>5)
</p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Unfortunately, I don’t have a figure for the random forest model to explain the method clearer. But if we look at this example of a classification tree in figure 4, it might help visualize this method. The two advantages of this tree are the graphic interpretability, in which it is easier to understand compared to statistical methods. Another is their performance with “highly non-linear decision boundaries”. But the disadvantage is that the tree is subject to variance. If a miniscule change were to occur in the data, the whole tree could transform to something entirely different. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Based on the couple hundred of trees, the output is the “score function” that a household is calculated to be in poverty or not. So, each tree predicts the status for a household. According to World Bank, Random Forest is a good predictor of poverty, and sometimes it is better than current methods. It is not the most accurate method, but it is more robust and does not make large prediction errors. Overall, Random Forest is a simple, automated method to take advantage of and can be used as a complement to other methods. [10]

### Discussion

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The two methods I selected, SAE & RF, are complimentary towards each other in regard to my research question. SAE doesn’t seem to rely only on census data, although that type of data is mostly used in the technique. The advantages of SAE include: design unbiased and design consistent, and it does not require model assumptions. The method performs well under complex sample designs and it includes informative sampling. However, the method is inefficient when dealing with small populations, and it is hard to produce results for non-sampled areas. For RF, the predictive performance of this method is able to compete with the best machine learning algorithms. And, it is very versatile as the model can be applicable for a variety of needs. But in my research question I am only looking at predictors of poverty. Other advantages of RF are that there is little pre-processing needed, and we can split the process into multiple machines to run. This is called parallelization, where we can cut down the processing time. But some disadvantages are: Random forest models are not that interpretable, the amount of data trees take can take up space, and it may tend to overfit. Overall, these two techniques can bring the best out of each other when used together. There might be, of course, a method more accurate. But, I am looking for an efficient method that lower-middle income countries can use while also keeping the quality and accuracy of the results intact. The research gap that I hope researchers will start to take notice of is the lack of data on SAE and RF together. There are plenty articles that deal with each method separately, but I think we should start to look for combinations of methods, as mentioned earlier, to bring the best out of both methods. Thus, it increases efficiency, accuracy, mapping, and estimates while keeping the cost and resources used low.

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
