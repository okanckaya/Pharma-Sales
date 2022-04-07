# Pharma Sales Prediction

In this project, which was prepared within the scope of the bootcamp organized with the partnership of **Kodluyoruz** and **Patika.dev** and, sponsored by **Eczacıbaşı VitrA**, it is aimed to estimate the expected sales values in the January-April 2021 range over the medicine sales prices from January 2017 to January 2021.

<img width="590" alt="Screen Shot 2022-03-24 at 17 31 24" src="https://user-images.githubusercontent.com/71854717/159939227-33be5655-72c1-47b5-bd6f-768a6dce2d02.png">

The data used in the project have been provided by **Eczacıbaşı Bilişim** through private interviews and there is no open access to the data.

In the main data set, only the ***product group***, the ***province*** where the sale was made, the ***time*** of the sale and the ***quantity*** are available.

<img width="386" alt="image" src="https://user-images.githubusercontent.com/71854717/161051504-da65916a-0fa2-4051-9834-6a90d26f9c00.png">

Within the scope of this repo, a prediction model was developed for the **Product  X**, which is a prostate product developed for male patients over the age of 60.

Since it is very difficult to predict the output with the existing input variables in the data set, it is clear that new parameters should be added for the product. Considering what might be effective in the sale of a product sold to male patients over 60 years of age, it was thought that adding the following parameters to the data set would have positive effects in terms of giving better results for the prediction model.
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

## Libraries 
<img width="656" alt="Screen Shot 2022-03-31 at 16 02 05" src="https://user-images.githubusercontent.com/71854717/161060859-e61970d2-7b62-4145-b7b5-4c1bc79ba44f.png">

