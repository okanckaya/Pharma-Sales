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

## Results for Dataset II:

|Model|Mean Absolute Error \(Train)|Mean Absolute Error \(Test)|Mean Squared Error \(Train)|Mean Squared Error \(Test)|Root Mean Squared Error \(Train)|Root Mean Squared Error \(Test)|R2 \(Train)|R2 \(Test)|Coefficient of Variance \(Train)|Coefficient of Variance \(Test)|
|---|---|---|---|---|---|---|---|---|---|---|
|Random Forest|14\.38|123\.40|911\.98|49935\.27|30\.20|223\.46|0\.99|0\.76|0\.13|0\.89|
|Gradient Boosting|46\.39|122\.93|4764\.64|51337\.29|69\.03|226\.58|0\.961|0\.75|0\.29|0\.90|
|Light GBM|24\.38|128\.33|1778\.85|52883\.60|42\.18|229\.96|0\.99|0\.74|0\.18|0\.91|
|XGBoost|48\.283|125\.07|5255\.48|53109\.83|72\.49|230\.46|0\.96|0\.74|0\.30|0\.92|
|KNN|109\.11|149\.48|42007\.43|78282\.26|204\.96|279\.79|0\.68|0\.62|0\.86|1\.11|
|Decision Trees|0\.0|148\.51|0\.0|82173\.98|0\.0|286\.66|1\.0|0\.60|0\.0|1\.14|
|Gauss NB|73\.39|169\.01|13732\.46|174128\.58|117\.19|417\.29|0\.90|0\.15|0\.49|1\.66|
|Support Vector Machines|164\.74|194\.61|128576\.70|207988\.71|358\.58|456\.06|0\.02|-0\.01|1\.51|1\.81|
|Linear Regression|152\.25|192\.17|86302\.43|219131\.54|293\.77|468\.11|0\.34|-0\.06|1\.23|1\.86|

## Results for Dataset III:

|Model|Mean Absolute Error \(Train)|Mean Absolute Error \(Test)|Mean Squared Error \(Train)|Mean Squared Error \(Test)|Root Mean Squared Error \(Train)|Root Mean Squared Error \(Test)|R2 \(Train)|R2 \(Test)|Coefficient of Variance \(Train)|Coefficient of Variance \(Test)|
|---|---|---|---|---|---|---|---|---|---|---|
|XGBoost|53\.59|137\.20|6607\.52|71193\.18|81\.28|266\.82|0\.94|0\.65|0\.34|1\.06|
|Gradient Boosting|52\.81|133\.89|6172\.99|71790\.97|78\.56|267\.93|0\.95|0\.65|0\.33|1\.06|
|Light GBM|30\.52|154\.70|3203\.10|84267\.08|56\.59|290\.28|0\.97|0\.59|0\.23|1\.15|
|KNN|115\.54|159\.35|49217\.11|95121\.35|221\.84|308\.41|0\.62|0\.53|0\.93|1\.22|
|Random Forest|16\.91|146\.01|1562\.32|97838\.59|39\.52|312\.79|0\.98|0\.52|0\.16|1\.24|
|Decision Trees|0\.0|170\.90|0\.0|146731\.92|0\.0|383\.05|1\.0|0\.28|0\.0|1\.52|
|Gauss NB|79\.22|171\.76|15456\.82|174229\.46|124\.32|417\.40|0\.88|0\.15|0\.52|1\.66|
|Support Vector Machines|163\.26|193\.92|127036\.58|207198\.18|356\.42|455\.19|0\.03|-0\.00|1\.49|1\.81|
|Linear Regression|150\.06|189\.58|86550\.57|216157\.12|294\.19|464\.92|0\.33|-0\.05|1\.23|1\.85|

## Results for Dataset IV:



Since the Random Forest, Decision Trees, Gradient Boosting and XGBoost algorithms  give the best results with *Dataset 5* than other algorithm-dataset combinations, grid search was performed to find the best possible result with these algorithm:
