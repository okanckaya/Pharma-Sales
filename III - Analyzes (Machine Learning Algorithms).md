# Creating Different Sub Datasets:

|Dataset # |Period|Province|Month|Year|Season|BigCity|Region|StockMarket|DolarB|DolarS|CPI(Year)|CPI(Month)|Male|Male_Province|Male_Rural|Trends_Eczacıbaşı|Trends_Prostat|Med_Deg|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Dataset I|+|+|+|+|+|+|+|+|+|+|+|+|+|+|+|+|+|+|
|Dataset II|-|+|+|+|+|+|+|+|-|+|+|+|+|+|-|+|+|+|
|Dataset III|-|-|+|+|+|+|+|+|-|+|+|+|+|+|-|+|+|+|
|Dataset IV|-|+|+|+|+|+|+|-|-|+|+|+|+|+|-|+|+|+|
|Dataset V|-|+|+|+|+|+|+|-|-|+|+|+|-|+|-|+|+|+|

Since the distributions of the datas are quite different, the input parameters must be brought to the same scale in order for the results to be more reliable. Therefore, in this section, the training and test data  are scaled to scatter around 0, but 2020 datas:

# Machine Learning Algorithms:

Machine Learning algorithms used in these project are:

  * Linear Regression
  * KNN
  * XGBoost
  * Light GBM
  * Random Forest
  * Support Mector Machines
  * Gauss NB
  * Decision Trees
  * Gradient Boosting





Since the Random Forest, Decision Trees, Gradient Boosting and XGBoost algorithms  give the best results with *Dataset 5* than other algorithm-dataset combinations, grid search was performed to find the best possible result with these algorithm:
