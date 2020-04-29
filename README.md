# Restaurant.visit.prediction:

### Description of Dataset    
 * The data set consisted of **3651** rows and **2** cloumns
 * The data showed number of visits in a restaurant each day for 3651 consecutive days.
 
### Data Cleaning  
 * Data exploration was done to find any missing values.
 * No missing values were found , but two rows consisted of negative number of visits.
 * These rows were removed.
 * The number of visitors were converted into whole numbers.
 
 ### Bivariate EDA
 * A bit of bivariate visualization was done to find any correlations
 * Finally, it was seen how much the given features correlated with the target feature('_vists_') 
 
 ### Feature Engineering and selection
 * The data stamp data was used to generate features such as day of the week,month and year.
 * Such features can be potential variables for prediction of visits.
 * Month and Year were found to correlate highly with number of visits.
 
 ### Building a predictive model  
 * Given data was split into test and train data.
 * The models chosen for prediction were:
   1. RandomForestRegressor
   2. AdaBoostRegressor
   3. BaggingRegressor
   4. SVR
   5. LinearRegression
   6. KneighboursRegressor  
  * Out of these SVR was selected since it gave least rmse value of **0.255**  
  * The predicted number of visit a day ahead was **31**
