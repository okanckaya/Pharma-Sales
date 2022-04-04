# Data Types 

dsadasdsd

# Heat Map

![image](https://user-images.githubusercontent.com/71854717/161548353-c06258a2-ac50-40f0-af19-beff196ca4c2.png)

# Outliers

![image](https://user-images.githubusercontent.com/71854717/161548548-27cc36c1-9847-4b7d-9bbd-247f6bf2a962.png)

# Dealing with Variables:

 * CPI(Year) and Borsa features show high correlation with each other. Beacuse of that the feature (Borsa) which correlates weaker with "Quantity" got eliminated.
 * DolarB and DolarS features show high correlation with each other. Beacuse of that one of them (DolarB) got eliminated.
 * Since the predictions are desired to be made without Province variable it's also got eliminated.
 * Since te Season variable also shows weak correlation with Quantity, it's also got eliminated.
 * Since Male, Male_Province and Male_Rural almost indicates the same thing, Male and Male_Rural variables eliminated due to lower correlation with Quantity.

# Giving Back products:

|index|Period|Province|Month|Year|Season|BigCity|Region|StockMarket|DolarB|DolarS|CPI\(Year)|CPI\(Month)|Male|Male\_Province|Male\_Rural|Trends\_Eczacıbaşı|Trends\_Prostat|Med\_Deg|Quantity|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|1315|2018-05-01 00:00:00|Gümüşhane|5|2018|spring|0|BS|2\.999|4\.4342|4\.4422|12\.15|1\.62|84585\.0|52299\.0|32286\.0|0|0|15\.2|-2\.0|
|2584|2019-09-01 00:00:00|Bilecik|9|2019|fall|0|MA|3\.07|5\.7047|5\.715|9\.26|0\.99|61485\.0|92273\.0|20978\.0|0|0|19\.2|-6\.0|
|2588|2019-09-01 00:00:00|Çanakkale|9|2019|fall|0|MA|3\.07|5\.7047|5\.715|9\.26|0\.99|1216490\.0|163780\.0|108566\.0|0|0|23\.4|-1\.0|
|2595|2019-09-01 00:00:00|Erzurum|9|2019|fall|1|EA|3\.07|5\.7047|5\.715|9\.26|0\.99|185788\.0|380779\.0|0\.0|0|0|14\.5|-22\.0|
|2612|2019-09-01 00:00:00|Kırıkkale|9|2019|fall|0|CE|3\.07|5\.7047|5\.715|9\.26|0\.99|152694\.0|132337\.0|52761\.0|0|38|20\.7|-7\.0|
|2620|2019-09-01 00:00:00|Mardin|9|2019|fall|1|SE|3\.07|5\.7047|5\.715|9\.26|0\.99|542072\.0|916076\.0|0\.0|0|0|25\.8|-4\.0|

|Year|Month|Province|BigCity|StockMarket|DolarB|DolarS|CPI\(Year)|CPI\(Month)|Male|Male\_Province|Male\_Rural|Trends\_Eczacıbaşı|Trends\_Prostat|Med\_Deg|Quantity|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|2018|5|Gümüşhane|0|2\.999|4\.4342|4\.4422|12\.15|1\.62|84585\.0|52299\.0|32286\.0|0|0|15\.2|-2\.0|
|2019|9|Bilecik|0|3\.07|5\.7047|5\.715|9\.26|0\.99|61485\.0|92273\.0|20978\.0|0|0|19\.2|-6\.0|
|2019|9|Erzurum|1|3\.07|5\.7047|5\.715|9\.26|0\.99|185788\.0|380779\.0|0\.0|0|0|14\.5|-22\.0|
|2019|9|Kırıkkale|0|3\.07|5\.7047|5\.715|9\.26|0\.99|152694\.0|132337\.0|52761\.0|0|38|20\.7|-7\.0|
|2019|9|Mardin|1|3\.07|5\.7047|5\.715|9\.26|0\.99|542072\.0|916076\.0|0\.0|0|0|25\.8|-4\.0|
|2019|9|Çanakkale|0|3\.07|5\.7047|5\.715|9\.26|0\.99|1216490\.0|163780\.0|108566\.0|0|0|23\.4|-1\.0|

# Visualization

Bar plot of Quantity-Region for three years period.

![image](https://user-images.githubusercontent.com/71854717/161552119-7cf74366-ec57-4bb5-958e-b8197609c8e1.png)

![image](https://user-images.githubusercontent.com/71854717/161552172-db2627c9-3046-496e-967a-82da105b30da.png)

![image](https://user-images.githubusercontent.com/71854717/161552229-25eb3e3f-0be6-461c-9c8f-6b1771e339d5.png)

![image](https://user-images.githubusercontent.com/71854717/161552281-89d45e8a-0b9e-42dd-a738-41ab8ebe9033.png)

It can be seen that from the year 2017 to 2019 Product X sold more every year except the excessive decrease on 08-2019 and 09-2019. As a result of the researches, it was thought that a product group similar to Product X was recalled from the market.

![image](https://user-images.githubusercontent.com/71854717/161552354-cacab802-8fb9-4679-964d-ba99d3f8b644.png)

As can be seen from the graph above, an increasing trend is observed in the sales of product X.

![image](https://user-images.githubusercontent.com/71854717/161552681-3d128146-bc07-4eda-afe4-8cbadcfe6489.png)

The sudden decrease mentioned above can be seen quite clearly in this chart.

|index|Province|Quantity|
|---|---|---|
|77|İstanbul|100631\.0|
|5|Ankara|43474\.0|
|29|Gaziantep|35620\.0|
|78|İzmir|32752\.0|
|44|Konya|25282\.0|
|9|Aydın|24297\.0|
|0|Adana|23507\.0|
|61|Samsun|17604\.0|
|41|Kayseri|17209\.0|
|6|Antalya|16949\.0|

![image](https://user-images.githubusercontent.com/71854717/161552905-ab03f754-caaa-4cda-bd37-e9d5a47b6f72.png)

Bar plot of Quantity-Province for three-year period. It can be seen that densely populated metropolitan areas like Istanbul, Ankara, Gaziantep etc. are on the top of the most-sold list.

|index|Province|Year|Quantity|
|---|---|---|---|
|309|İstanbul|2018|31410\.0|
|21|Ankara|2018|14295\.0|
|117|Gaziantep|2018|11547\.0|
|313|İzmir|2018|10303\.0|
|177|Konya|2018|9221\.0|
|37|Aydın|2018|7996\.0|
|1|Adana|2018|7180\.0|
|165|Kayseri|2018|6604\.0|
|25|Antalya|2018|5999\.0|
|81|Bursa|2018|5458\.0|

|index|Province|Year|Quantity|
|---|---|---|---|
|310|İstanbul|2019|39225\.0|
|22|Ankara|2019|14277\.0|
|118|Gaziantep|2019|12437\.0|
|314|İzmir|2019|11983\.0|
|178|Konya|2019|9009\.0|
|38|Aydın|2019|8534\.0|
|2|Adana|2019|7709\.0|
|246|Samsun|2019|7145\.0|
|202|Manisa|2019|6443\.0|
|166|Kayseri|2019|6336\.0|
