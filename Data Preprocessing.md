Since the main data set contains only three variables (period, province and quantitiy), it is obvious that new variables must be added to the data set in order to develop a suitable forecasting model. As stated in the Read.me file, when the variables that may affect the sales of a product group sold to male patients aged 60 and over are considered, the following variables come to mind:
  * Province and time based air temperature
  * Season
  * Whether the province is a big city or not
  * Region (Marmara, Black Sea etc.)
  * Stock market
  * Dolar exchange rate
  * Consumer Price Index (CPI) for year and month
  * Total male population in the province
  * Total male population in the rural areas
  * Google Trend data for "Eczacıbaşı" searchs
  * Google Trend data for "prostate" searchs

In order to approach the data in a holistic manner on a provincial basis, first of all, the total sales quantity in each province in the specified periods were combined. As a result of the total quantity, it was seen that no sales were made in the specified time intervals in some provinces. For this reason, **0**  is entered in the quantity column for the specified province and time periods.

`ProductX['Quantity'] = ProductX['Quantity'].fillna(0)`

At the same time, the 13th month information in the data set containing the province-based lowest, average and highest air temperatures between January 2017 and April 2020, which was obtained from the General Directorate of Meteorology, was deleted from the data set, considering it to be incorrect.

`df_heat = df_heat[df_heat.Month != 13]`

|index|Period|Province|Month|Year|Season|BigCity|Region|Borsa|DolarB|DolarS|CPI\(Year)|CPI\(Month)|Male|Male\_Province|Male\_Rural|Trends\_Eczacıbaşı|Trends\_Prostat|Quantity|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|0|201701|Adana|1|2017|winter|1|ME|2,379|3,7468|3,7536|9,22|2,46|1101973|1101973|0|6|28|910\.0|
|1|201701|Adıyaman|1|2017|winter|0|SE|2,379|3,7468|3,7536|9,22|2,46|307819|203955|103865|0|0|44\.0|
|2|201701|Afyon|1|2017|winter|0|AE|2,379|3,7468|3,7536|9,22|2,46|354456|207099|147357|0|24|236\.0|
|3|201701|Ağrı|1|2017|winter|0|EA|2,379|3,7468|3,7536|9,22|2,46|281105|158643|122462|0|0|126\.0|
|4|201701|Aksaray|1|2017|winter|0|CE|2,379|3,7468|3,7536|9,22|2,46|197601|130684|66917|0|0|70\.0|
|5|201701|Amasya|1|2017|winter|0|BS|2,379|3,7468|3,7536|9,22|2,46|161792|115224|46568|0|48|214\.0|
|6|201701|Ankara|1|2017|winter|1|CE|2,379|3,7468|3,7536|9,22|2,46|2657519|2657519|0|22|37|1288\.0|
|7|201701|Antalya|1|2017|winter|1|ME|2,379|3,7468|3,7536|9,22|2,46|1176407|1176407|0|0|14|475\.0|
|8|201701|Ardahan|1|2017|winter|0|EA|2,379|3,7468|3,7536|9,22|2,46|50837|20082|30755|0|0|12\.0|
|9|201701|Artvin|1|2017|winter|0|BS|2,379|3,7468|3,7536|9,22|2,46|84508|50365|34142|0|100|27\.0|
