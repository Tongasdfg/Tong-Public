# Tong-Public 

### Description
This is a R based model that helps to predict GDP. This is also a group project. Emma Weber and I finished this project together in 2017. 

### Project Background
After the world war II, some countries recovered quickly and gradually became development countries. However, there are still many developing countries today. We want to analyze the data and build a solid model to find which variables are correlated to boost the economy. We pick GDP, the most representative variable in the economy, as our Y variable. We assume that GDP are correlated to the natural resources, infrastructure, population and technology.  As a result, we pick agriculture, export, foreign investment, imports, industry, inflation rate, population, debt, fertility rate and computer as our x variables to start with. 

### Procedures
The first thing I did is to create another table and only selected the variables we need. Because most of the variables have strange names, then I changed names for these variables. In addition, even though all of our variables should be numeric for linear regression, variables except agriculture in the original data set are all factors. I decided to translate these factor variables into numeric variables. Finally, I removed all the na in the data set so we can run the best subset.

### Hypothesis
H0: GDP is not correlated to any of the x variables in our model which include natural resources, infrastructure, population and technology. 
Ha: GDP is correlated to at least one of the x variables in our model which include natural resources, infrastructure, population and technology.

### Flaws
Because we are building several models here, we have Type I error. So we will decrease the p value. Instead of using p value 0.05, we will use 0.05/6 (we build 6 models) as the p value.

### Conclusion
Our final model is log(GDP)=7.96+0.27*(log(debt))+0.62*(log(population))-0.037*(agriculture). Almost 82% of the data points can be explained by this model. 
If we go back to our hypothesis, log(GDP) is correlated with log(debt), log(population), and agriculture. 

### Reference
The data set comes from the book Practicing Statistics Guided Investigations for 2th, Shonda Kuiper and Jeff Sklar, Jan 6, 2012.



