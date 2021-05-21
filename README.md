# Regression
### from data.gov.in
The dataset contains the information about the taxation in the west zone of Surat for some chosen wards from the year 2004 to 2015.
### Problem Statement-
For the given dataset our framed regression problem is to predict the total recovery which is dependent on demand. We have observed that ward no and year attribute are not related to Total recovery so we took-
Independent attribute: Demand
Dependent attribute: Total Recovery.
Both the terms are highly correlated that can be seen in the following correlation matrix. The values for the attributes are in crores.
![correlation matrix](https://github.com/Ashwani-Varshney/regression/blob/main/corr.jpg)

|Library|	Function|	Usage|
|-------|------|--------|
|Pandas|	read_csv|	to read the dataset|
|NumPy|	Sqrt|	to calculate square root|
|Seaborn|	heatmap, distmap|	to visualize relationship b/w dependent & independent variable|
|sklearn.model_selection|	train_test_split|	to partition the dataset|
|sklearn.metrics|	mean_absolute_error, mean_squared_error|	to find mean squared error, mean absolute error and root mean squared error|
|sklearn.linear_model|	LinearRegression|	to fit linear regression on dataset|
|matplotlib|	Pyplot|	to visualize regression results and obtain relationship b/w dependent & independent variable|


Result and Interpretation-
-

![Regression plot](https://github.com/Ashwani-Varshney/regression/blob/main/plot1.jpg) 
-

The actual and predicted values are quite similar to each other, as observed from the above graph.

![Regression plot](https://github.com/Ashwani-Varshney/regression/blob/main/plot.jpg) 
-
From the above graph we can see that the linear model fits the data quite well.
Mean Absolute Error: 0.8357969545192269
Mean Squared Error: 2.0625294895366375
Root Mean Squared Error: 1.4361509285366345
R2 value: 0.9601400116543154

We defined the R-squared value, as the fraction by which the variance of the errors is less than the variance of the dependent variable. Since the R-squared value is nearly 1, this implies a very low standard deviation, we can say that the model is a good fit for the data.
