# Joseph Goerner


# Clustering--Project


# Project Planning 

I as a junior data scientest was given the task to find logerror in the 2017 housing data. I first asked a question about logerror, what is logerror?
I came up with the formula >`logerror` = log (Zestimate) − log (ActualSalePrice), and off to the data I went, I followed my mvp steps and steps to reproduce and spent the last 5 days digging and cleaning to find any new information I could find I created a model that perfomed %0.0003 improvment over base line. I just continued to think and work until my deadline approched. 


# Steps to reproduce 
<div class="alert alert-block alert-warning">    

<span style="color:maroon;"> 
    <div class="alert alert-block alert-warning">    
<span style="color:maroon;"> <strong>

Events in sequence 
1. Import , from the codeup sql and use your log information.
2. Acquire Data
3. Clean, Prep and Split Data
4. Explore Data 
 * Hypothesis Testing
6. Evaluation of Data 
7. Modeling
 * Mvp, Identify Baseline 
 * Train and Validate 
 * We Test our best 
8. Conclusion and Recomindations 
</span>
</div>
</strong>

# Data Dictionary 
  
  
 -LA'- one of the dummy files I created for county 
 
 -Orange - one of the dummy files I created for county
 
 -Ventura - one of the dummy files I created for county
 
 -fips - The tax codes for the county

 -latitude - map cordinates for the countys 
 
 -longitude'- map cordinates for the countys 
 
 -sqft - house square feet 
 
 -lot_sqft- area around the house sqft 
 
 -zip_code- the zipcode for the houses in the counties 
 
 -property_quality'- how the house holds up in terms of quality 
 
 -home_age' - How long the house has been since it has been built 
 
 -logerror' - `logerror` = log (Zestimate) − log (ActualSalePrice)
 
 -structure_value'- the actual home or structure value 
 
 -bedrooms - the number on how many bedrooms there are 
 
 -bathrooms'- the number on how many bathrooms there are 
 
 -land_value - the value of the land in a dollar amount 
 
 -structure_dollar_per_sqft'- the mean cost of how much a house is worth per sqft 
 
 -land_dollar_per_sqft'- the mean cost of how much the area around the house cost 
 
 -bed_bath_ratio', bed and bath ratio that is used with outliers removed
 
 -avgqualityavgage', - a home of avrage quality 
 
 -poor_quality_old_age', a poor quality home 
 
 -avq_quality_young_age', a avg quality home, but a young age life 
 
 -avg_quality_old_age', a ave quality home, but old age life 
 
 -bestest' - the bestested for my clusters and age specimen



<h3> <span style="color:maroon;">
<h3> Executive Summary: </span> </h3>  
<h3><span style="color:maroon;">Project Goals- To identify drivers of error in the Zestimate in order to improve accuracy of predicting home values, with the help of Ml and clustering models. </h3>

>`logerror` = log (Zestimate) − log (ActualSalePrice)  

<h3><span style="color:maroon;">In this presention I will attack and perform the heavy proccess of Cluster analysis on the logerror values from the year of 2017, to predict future homeprices. I will also be searching for the key drives of logerror, This turned out to be </h3>   
    


  <span style="color:black;">   

- 'sqft',
-'lot_sqft',
- 'bedrooms',
- 'bathrooms',
- 'structure_dollar_per_sqft',
- 'land_dollar_per_sqft',
- 'poor_quality_old_age',
- 'avq_quality_young_age'
-'longitude'
    </span>
<h3><span style="color:maroon;"> I created a ols regressor model with a %0.0003 effective improvement over my baseline so I as a data scientist would recommend further analysis with my model.</h3> 

BASELINE:
              
              RMSE using Median
              Train/In-Sample: 0.164122
              Validate/Out-of-Sample: 0.166928
              
              
    RMSE for OLS using LinearRegression
    
    Test/Out-of-Sample Performance: 0.161775
    
##  FIPS 
<span style="color:black;">

* Los Angeles County, California (6037)
* Orange County, California (6059)
* Ventura County, California (6111)
  
# <span style="color:maroon;"> Hypotheses </span>

1.Fail to reject the null hypothesis // home_age and logerror.
There is a linear relationship.
Although, it is a negative weak one.
    
2.Reject null statment: No correlation between lot_sqft and logerror.
There is a linear relationship.
Although, it is a positive weak one.

3.Fail to reject the null hypothesis // No correlation between home_value and logerror.

    
    
-LA:  0.014516765820273388

-Orange:  0.01786707488534417

-Ventura: 0.013923148212340804 

4. All three counties rejected the null hypothiesis


