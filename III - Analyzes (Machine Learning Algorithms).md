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
|Random Forest|14\.605555555555556|123\.83072832369942|929\.0028384920638|52244\.23482751445|30\.479547872172642|228\.5699779662991|0\.9929117933920164|0\.7460923567182582|0\.1281753884268956|0\.9092386303953971|
|XGBoost|48\.66967881855274|125\.17990720396097|5238\.314477991906|54330\.23175224312|72\.37620104697335|233\.08846336153817|0\.9600321400977985|0\.7359543852310794|0\.3043630345490957|0\.9272129134083418|
|Light GBM|24\.594531786689256|134\.2146598681188|1774\.2159334351595|54599\.99149253098|42\.12144267988882|233\.66641070665457|0\.9864628948564054|0\.7346433494749827|0\.1771329515529038|0\.9295119557287281|
|Decision Trees|0\.0|162\.4242774566474|0\.0|69386\.90982658959|0\.0|263\.41395146534967|1\.0|0\.6627787389969844|0\.0|1\.0478460145483652|
|KNN|109\.67619047619048|151\.3741040462428|41215\.4875|82605\.05817341042|203\.01597843519608|287\.41095694738294|0\.6855296036307414|0\.5985383705358467|0\.853741400690359|1\.1433047646091095|
|Gauss NB|77\.34871031746032|169\.35375722543353|15143\.125496031746|174132\.07976878612|123\.0574073188272|417\.2913607646175|0\.8844593388102827|0\.15371588578505302|0\.5174922885354815|1\.6599617706284882|
|Support Vector Machines|165\.3171781967516|195\.71165125539488|129051\.18563801984|208605\.8184697156|359\.2369491547603|456\.73385956125|0\.01535126814863319|-0\.013826921140195125|1\.5106961457667498|1\.8168618320639838|
|Linear Regression|152\.00605763763747|192\.5579683625021|86183\.71618314415|216017\.35650766047|293\.5706323581161|464\.7766737989983|0\.3424261355955327|-0\.0498470899209329|1\.2345501314862077|1\.8488556987437674|



Since the Random Forest, Decision Trees, Gradient Boosting and XGBoost algorithms  give the best results with *Dataset 5* than other algorithm-dataset combinations, grid search was performed to find the best possible result with these algorithm:
