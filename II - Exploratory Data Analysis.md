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
