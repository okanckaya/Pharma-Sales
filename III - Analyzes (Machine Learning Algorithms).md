# Creating Different Sub Datasets:

|Dataset # |Period|Province|Month|Year|Season|BigCity|Region|StockMarket|DolarB|DolarS|CPI(Year)|CPI(Month)|Male|Male_Province|Male_Rural|Trends_Eczacıbaşı|Trends_Prostat|Med_Deg|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Dataset I|-|+|+|+|+|+|+|+|+|-|+|+|+|+|+|+|+|+|
|Dataset II|-|+|+|+|+|+|+|+|+|-|+|-|+|+|+|+|+|+|
|Dataset III|-|+|+|+|+|+|+|+|-|-|+|+|+|+|+|+|+|+|
|Dataset IV|-|+|+|+|-|+|+|+|+|-|+|+|+|+|+|+|+|+|
|Dataset V|-|+|+|+|-|+|+|+|-|-|+|-|+|+|+|+|+|+|

Since the variables month, year and season are produced depending on the period variable, the variable period is removed from all data sets. At the same time, since the "Dollar B" and "Dollar S" variables showed the same correlation value with the "Quantity" variable, the "Dollar S" variable was removed from all data sets. Since the "Season", "Dollar B" and "CPI (Month)" variables are the variables that show the lowest correlations with the "Quantity" variable, sub-datasets of all three subtractions were created separately.

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

|Model|Mean Absolute Error \(Train)|Mean Absolute Error \(Test)|Mean Squared Error \(Train)|Mean Squared Error \(Test)|Root Mean Squared Error \(Train)|Root Mean Squared Error \(Test)|R2 \(Train)|R2 \(Test)|Coefficient of Variance \(Train)|Coefficient of Variance \(Test)|2020-01 Prediction|2020-02 Prediction|2020-03 Prediction|2020-04 Prediction|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Gradient Boosting|47\.30|117\.96|4932\.12|49004\.20|70\.22|221\.36|0\.9623|0\.7618|0\.29|0\.88|19838|19845|19303|17104|
|XGBoost|48\.66|125\.17|5238\.31|54330\.23|72\.37|233\.08|0\.96005|0\.7359|0\.307|0\.92|20370|20317|19996|17672|
|Light GBM|24\.59|134\.21|1774\.21|54599\.99|42\.12|233\.66|0\.9864|0\.7346|0\.17|0\.92|20495|20709|20390|18782|
|Random Forest|14\.42|128\.37|945\.99|56167\.64|30\.756|236\.99|0\.9927|0\.7270|0\.12|0\.94|22118|22500|21930|20379|
|KNN|108\.69|150\.91|40081\.071|82818\.57|200\.20|287\.78|0\.69418|0\.5975|0\.84|1\.14|17062|17162|17256|17332|
|Decision Trees|0\.0|169\.42|0\.0|84340\.34|0\.0|290\.41|1\.0|0\.59010|0\.0|1\.15|19107|20268|9661|18644\.0|
|Gauss NB|75\.37|168\.49|14568\.82|172938\.69|120\.70|415\.85|0\.88|0\.15|0\.50|1\.65|15421|15420\.0|10491\.0|10617\.0|
|Support Vector Machines|164\.88|194\.48|128800\.23|207938\.79|358\.88|456\.00|0\.01|-0\.01|1\.50|1\.81|11078|11464|11058|11134|
|Linear Regression|151\.97|192\.00|86209\.79|217068\.24|293\.61|465\.90|0\.34|-0\.05|1\.23|1\.854|20490|20755|20006|17618|

## Results for Dataset II:

|Model|Mean Absolute Error \(Train)|Mean Absolute Error \(Test)|Mean Squared Error \(Train)|Mean Squared Error \(Test)|Root Mean Squared Error \(Train)|Root Mean Squared Error \(Test)|R2 \(Train)|R2 \(Test)|Coefficient of Variance \(Train)|Coefficient of Variance \(Test)|2020-01 Prediction|2020-02 Prediction|2020-03 Prediction|2020-04 Prediction|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Random Forest|14\.44|118\.54|884\.64|46260\.48|29\.74|215\.08|0\.99|0\.78|0\.13|0\.86|21356\.66|21692\.95|21013\.5|19596\.78|
|Gradient Boosting|46\.3|118\.55|4726\.8|48730\.72|68\.75|220\.75|0\.96|0\.76|0\.29|0\.88|20623\.97|20713\.19|20300\.06|17872\.67|
|XGBoost|48\.12|123\.2|5145\.2|54093\.88|71\.73|232\.58|0\.96|0\.74|0\.3|0\.93|19964\.22|20136\.52|19895\.7|17599\.29|
|Light GBM|24\.51|135\.15|1760\.28|54688\.66|41\.96|233\.86|0\.99|0\.73|0\.18|0\.93|19958\.4|20138\.76|20064\.19|18033\.81|
|KNN|105\.29|149\.05|35510\.87|81472\.01|188\.44|285\.43|0\.73|0\.6|0\.79|1\.14|16220\.0|16869\.8|16893\.8|17663\.2|
|Decision Trees|0\.0|176\.44|0\.0|91837\.72|0\.0|303\.05|1\.0|0\.55|0\.0|1\.21|20345\.0|21034\.0|20819\.0|20406\.0|
|Gauss NB|73\.66|168\.55|14253\.38|173738\.4|119\.39|416\.82|0\.89|0\.16|0\.5|1\.66|15742\.0|15292\.0|11096\.0|12352\.0|
|Support Vector Machines|163\.67|193\.98|128121\.25|207707\.68|357\.94|455\.75|0\.02|-0\.01|1\.51|1\.81|11093\.4|11470\.76|11033\.45|11123\.8|
|Linear Regression|151\.93|192\.7|86237\.45|216741\.0|293\.66|465\.55|0\.34|-0\.05|1\.23|1\.85|20997\.34|20731\.95|20113\.4|17868\.8|

## Results for Dataset III:

|Model|Mean Absolute Error \(Train)|Mean Absolute Error \(Test)|Mean Squared Error \(Train)|Mean Squared Error \(Test)|Root Mean Squared Error \(Train)|Root Mean Squared Error \(Test)|R2 \(Train)|R2 \(Test)|Coefficient of Variance \(Train)|Coefficient of Variance \(Test)|2020-01 Prediction|2020-02 Prediction|2020-03 Prediction|2020-04 Prediction|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Gradient Boosting|47\.09|118\.86|4963\.47|49398\.33|70\.45|222\.26|0\.96|0\.76|0\.3|0\.88|20419\.33|20457\.5|19999\.87|17323\.89|
|Random Forest|14\.46|127\.07|834\.81|52536\.6|28\.89|229\.21|0\.99|0\.74|0\.12|0\.91|21345\.69|21667\.64|21273\.88|19850\.25|
|XGBoost|48\.26|122\.35|5237\.2|54004\.4|72\.37|232\.39|0\.96|0\.74|0\.3|0\.92|20163\.66|20181\.76|19760\.31|17155\.01|
|Light GBM|24\.97|136\.65|1853\.92|55288\.1|43\.06|235\.13|0\.99|0\.73|0\.18|0\.94|19482\.46|19846\.17|18787\.74|16989\.21|
|Decision Trees|0\.0|157\.46|0\.0|67169\.99|0\.0|259\.17|1\.0|0\.67|0\.0|1\.03|20156\.0|20737\.0|22412\.0|20705\.0|
|KNN|107\.96|149\.36|39652\.08|76778\.91|199\.13|277\.09|0\.7|0\.63|0\.84|1\.1|17536\.0|17339\.6|16776\.8|15843\.6|
|Gauss NB|73\.36|169\.36|14003\.71|173117\.56|118\.34|416\.07|0\.89|0\.16|0\.5|1\.66|15678\.0|15639\.0|10553\.0|10560\.0|
|Support Vector Machines|164\.41|192\.89|128601\.37|207221\.75|358\.61|455\.22|0\.02|-0\.01|1\.51|1\.81|11042\.78|11443\.18|11018\.46|11124\.53|
|Linear Regression|152\.08|197\.59|86285\.68|221231\.3|293\.74|470\.35|0\.34|-0\.08|1\.24|1\.87|21608\.72|21039\.73|20657\.77|18565\.26|
## Results for Dataset IV:

|Model|Mean Absolute Error \(Train)|Mean Absolute Error \(Test)|Mean Squared Error \(Train)|Mean Squared Error \(Test)|Root Mean Squared Error \(Train)|Root Mean Squared Error \(Test)|R2 \(Train)|R2 \(Test)|Coefficient of Variance \(Train)|Coefficient of Variance \(Test)|2020-01 Prediction|2020-02 Prediction|2020-03 Prediction|2020-04 Prediction|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Gradient Boosting|47\.31|119\.21|4932\.13|48983\.66|70\.23|221\.32|0\.96|0\.76|0\.3|0\.88|20127\.41|19544\.31|19816\.33|19113\.32|
|Random Forest|14\.5|123\.22|852\.89|51278\.68|29\.2|226\.45|0\.99|0\.75|0\.12|0\.9|20639\.66|19612\.82|19684\.8|18661\.41|
|Light GBM|24\.77|132\.68|1821\.47|54072\.73|42\.68|232\.54|0\.99|0\.74|0\.18|0\.93|20409\.7|19445\.18|19923\.03|18701\.96|
|XGBoost|48\.67|125\.18|5238\.31|54330\.23|72\.38|233\.09|0\.96|0\.74|0\.3|0\.93|20045\.38|19418\.21|19695\.45|19036\.61|
|KNN|105\.18|150\.05|36517\.1|84894\.97|191\.09|291\.37|0\.72|0\.59|0\.8|1\.16|20050\.4|18272\.8|19368\.8|18831\.2|
|Decision Trees|0\.0|179\.63|0\.0|97565\.79|0\.0|312\.36|1\.0|0\.53|0\.0|1\.24|20325\.0|19232\.0|19913\.0|18222\.0|
|Gauss NB|70\.47|167\.87|13445\.08|173758\.42|115\.95|416\.84|0\.9|0\.16|0\.49|1\.66|26297\.0|24218\.0|24541\.0|19542\.0|
|Support Vector Machines|163\.76|194\.0|128004\.98|207518\.9|357\.78|455\.54|0\.02|-0\.01|1\.5|1\.81|11213\.24|10899\.62|10936\.81|10874\.08|
|Linear Regression|151\.98|192\.1|86210\.41|217042\.45|293\.62|465\.88|0\.34|-0\.05|1\.23|1\.85|19881\.02|18913\.78|19332\.04|19452\.77|

## Results for Dataset V:

|Model|Mean Absolute Error \(Train)|Mean Absolute Error \(Test)|Mean Squared Error \(Train)|Mean Squared Error \(Test)|Root Mean Squared Error \(Train)|Root Mean Squared Error \(Test)|R2 \(Train)|R2 \(Test)|Coefficient of Variance \(Train)|Coefficient of Variance \(Test)|2020-01 Prediction|2020-02 Prediction|2020-03 Prediction|2020-04 Prediction|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|Gradient Boosting|47\.22|119\.83|5014\.59|49085\.31|70\.81|221\.55|0\.96|0\.76|0\.3|0\.88|19697\.9|19784\.73|19036\.55|16368\.16|
|Random Forest|14\.41|122\.31|898\.39|53223\.17|29\.97|230\.7|0\.99|0\.74|0\.13|0\.92|21352\.73|21650\.65|21306\.65|19752\.97|
|XGBoost|47\.6|120\.58|5012\.72|53421\.45|70\.8|231\.13|0\.96|0\.74|0\.3|0\.92|20546\.77|20557\.82|20023\.5|17661\.66|
|Light GBM|24\.96|131\.78|1817\.78|53660\.93|42\.64|231\.65|0\.99|0\.74|0\.18|0\.92|19755\.06|19282\.18|19438\.06|17110\.59|
|KNN|97\.19|146\.53|29228\.71|76589\.99|170\.96|276\.75|0\.78|0\.63|0\.72|1\.1|16891\.4|17785\.2|16830\.0|16656\.8|
|Decision Trees|0\.0|160\.3|0\.0|80054\.12|0\.0|282\.94|1\.0|0\.61|0\.0|1\.13|19087\.0|19348\.0|20722\.0|19458\.0|
|Gauss NB|67\.82|168\.4|12642\.95|172542\.63|112\.44|415\.38|0\.9|0\.16|0\.47|1\.65|14467\.0|14877\.0|11283\.0|12002\.0|
|Support Vector Machines|161\.7|192\.04|126684\.17|206029\.24|355\.93|453\.9|0\.03|-0\.0|1\.5|1\.81|11321\.52|11724\.62|11238\.63|11013\.46|
|Linear Regression|152\.07|196\.61|86291\.24|221149\.16|293\.75|470\.26|0\.34|-0\.07|1\.24|1\.87|21575\.49|21018\.21|20781\.85|18209\.13|

As it can be seen that Random Forest and *Dataset 2*  give the best results. 

***MOVING AVERAGES***

Since the results obtained in the previous analyzes were not satisfactory, it was necessary to consider of adding new parameters to the dataset. In this section, three additional columns have been added to the main data set in order to better model the upward trend in sales data: Sales data of the previous month, sales data of three months ago, average sales quantity of the last three months.

Since the XGBOOST algorithm performs well in general and can work with missing data, it has been chosen in this section.

