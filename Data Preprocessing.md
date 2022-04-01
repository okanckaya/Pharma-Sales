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
