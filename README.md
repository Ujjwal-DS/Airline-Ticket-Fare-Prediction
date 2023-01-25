# Airline-Ticket-Fare-Prediction
•	The project aims to find out the best prices of the airplane tickets for the provided itenaries ,in order to make the air journey convenient for passengers so that more tickets can be booked which directly benefit the airlines such that flights may run on their full capacities.

•	This aim is being planned to fulfill by making a machine learning based regression model which when deployed can be able to find out the best prices for the future travels of any passenger.

•	This machine learning model is being planned to be worked on a dataset that is being provided by EaseMyTrip for a span of 2 months,2022.The dataset was divided into Economy and Business classes initially which was later merged into a single dataset and the further processes are being carried over it.

•	We have gone through various challenges while performing Data Cleaning from cleaning various columns containg unknown characters to changing their datatypes to the nature they need to be dealt with. While performing the same we have observed the stops column comprising of 0,1,2 and 2+ stops but when the column was being further analysed, it was found that the stops are missing for more than 1 stops,making that column not relevant.

•	We have tried to do Data manipulation by adding  a distance column from source to destination . But since as the stops were not giving the sufficient information ,simply adding the distance between source and destination airports may be of no use. As a result of which we have decided to not consider it for our future analysis.

•	Then we headed with the Exploratory Data Analysis where we did univariate,bivariate as well as multivariate analysis out of which we concluded many things about various airlines,ticket prices corresponding to both classes,no. of stops,source airport where we found that Vistara airways,Business classes,flights from Kolkata,single stop flights, are having the most expensive flight tickets.

•	We then headed with the Feature Engineering part where we made a new column called departure time  and arrival time being extracted from flight arrival and departure times making our analysis even easier to move with.

•	We then performed dummy encoding over our categorical features. No scaling was performed as we are left with only one numerical feature apart of target variable,sollowed by train test split.

•	Checking for assumptions being our next step where we found that there is high multicollinearity present as well as the residuals are not normal in nature. We further tried removing multicollinearity with the help of VIF but we found that there is moderate multicollinearity present.

•	Also the residuals for time_taken column was seen to follow the linearity and no other residual follow.

•	We then headed with base model model building followed with 7 other models from where we found that the Hyper-tuned Random Forest model  to be performing the best but because of significant difference between train-test RMSE ,it got overfitted. Also the algorithms were taking so much time to run. As  a result of which we headed with finding out the most significant features use RFE technique.

•	Again with the new selected features, we again headed with the building of all the 8 models.Now the algorithms were taking lesser time to run with significantly improved accuracy. 

•	We found that with the best features selected, Hyper-tuned Random Forest model to be performing as the best one with the overfitting being reduced.

# ScreenShot:

![image](https://user-images.githubusercontent.com/110291864/214470115-15bc576a-3db5-48be-bdc6-752d17a5edc7.png)

