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

## Result for Dataset I:

|Model|Mean Absolute Error \(Train)|Mean Absolute Error \(Test)|Mean Squared Error \(Train)|Mean Squared Error \(Test)|Root Mean Squared Error \(Train)|Root Mean Squared Error \(Test)|R2 \(Train)|R2 \(Test)|Coefficient of Variance \(Train)|Coefficient of Variance \(Test)|
|---|---|---|---|---|---|---|---|---|---|---|
|Gradient Boosting|47\.31|120\.33|4932\.13|49322\.01|70\.23|222\.09|0\.96|0\.76|0\.30|0\.88|
|Random Forest|14\.61|123\.83|929\.00|52244\.23|30\.48|228\.57|0\.99|0\.75|0\.13|0\.91|
|XGBoost|48\.67|125\.18|5238\.31|54330\.23|72\.38|233\.089|0\.960\.74|0\.304|0\.93|
|Light GBM|24\.59|134\.21|1774\.22|54599\.99|42\.12|233\.67|0\.99|0\.73|0\.18|0\.93|
|Decision Trees|0\.0|162\.42|0\.0|69386\.91|0\.0|263\.41|1\.0|0\.66|0\.0|1\.05|
|KNN|109\.68|151\.37|41215\.49|82605\.06|203\.02|287\.41|0\.69|0\.60|0\.85|1\.14|
|Gauss NB|77\.35|169\.35|15143\.13|174132\.08|123\.06|417\.29|0\.88|0\.15|0\.52|1\.66|
|Support Vector Machines|165\.32|195\.71|129051\.19|208605\.82|359\.24|456\.73|0\.02|-0\.01|1\.51|1\.82|
|Linear Regression|152\.01|192\.56|86183\.72|216017\.36|293\.57|464\.78|0\.34|-0\.05|1\.23|1\.85|



Since the Random Forest, Decision Trees, Gradient Boosting and XGBoost algorithms  give the best results with *Dataset 5* than other algorithm-dataset combinations, grid search was performed to find the best possible result with these algorithm:
