# Educational Data Visualizations and Predictive Analysis

![education.jpeg](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/Education.jpeg)


# Background

The predictive data analysis on the following pages seeks to investigate the relationship, if any, between various financial and socioeconomic factors and their impact on student achievement. We first began our investigation by acquiring student achievement data from the National Assessment of Educational Progress, which is an organization that measures what U.S. students know and can do in various subjects across the nation, in each individual state. This assessment is given every two years to a representative sample of students across the country. For our research purposes and initial data analysis, we narrowed down the data and looked at average reading and math scores in grades 4 and 8 across each of the 50 states during the 2013, 2015, and 2017 testing years.

 ![NAEP.jpeg](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/NCES.png)

After gathering the average score data from the NAEP, total revenue (federal and state sources), and total instructional spending from the United States Department of Education, we then collected financial data from the US Census Bureau on median household income and poverty rate for each of the 50 states.

Following the initial 3-year analysis, we decided to further our research and analysis by gathering more data and creating a machine learning model that could predict student achievement based on the factors that showed a correlation. 

Our mission: to find a correlation, or lack thereof, between these financial and socioeconomic variables and the impact on student achievement in order to better inform education policy makers and stakeholders in the future.


# Architecture Diagram
![Architecture_Diagram.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/Architecture_Diagram.png)


# Data Visualiztion

* Homepage
![Homepage1.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/Homepage1.png)

  ![Homepage2.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/Homepage2.png)


* State Analysis
![Dashboard_1.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/dashboard_1.png)


  ![Dashboard_2.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/dashboard_2.png)

* National Analysis
![scatterPlot.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/scatterPlot.png)

# Machine Learning Model
Through our initial analysis, we found a strong, linear correlation between poverty rate, median income, and student achievement. We used this knowledge to inform the development of our machine learning model. 

We gathered 9 total years of average score data from the NAEP in 4th and 8th grade math and reading. We then gathered additional data on poverty rate, median household income, and unemployment rate in each of the 50 states for the same corresponding years of data. Using this data, we analyzed approximately 20 different machine learning models to see which would perform best with our data and the 3 features we chose. Ultimately, we chose to use a Linear Regression model because it was the best fit for our data.

After testing and training the model, we gathered poverty rate, median household income, and unemployment rate data for every county in the United States in 2020. We used this data to make predictions on average scores in each of the four grades/subjects we analyzed. Through Flask and API, we developed a user-input model on our webpage that allows users to input their zip code and receive average score predictions based on the area they live in. In addition, we created another user-input form where customized poverty rates, incomes, and unemployment rates can be entered to predict average score data.

![ML_caro_1.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/ML_caro_1.png)

![ML_caro_1.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/ML_caro_2.png)

![Pred_by_county.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/Pred_by_county.png)

* National Analysis
![Pred_Try_yours.png](https://github.com/PeiDay/Student_Performance_Prediction/blob/main/static/images/Pred_Try_yours.png)


# Conclusion
As stated above, in our initial analysis we discovered that there was no apparent correlation between total revenue, instructional spending, and student achievement. However, we did find a significant, linear relationship between both poverty rate and median household income. Because of this, we decided to further our analysis and investigate the relationship between all socioeconomic factors (poverty rate, median household income, and unemployment rate) and student achievement.

Through our analysis, we found statistically significant evidence to suggest that a students’ socioeconomic status has an impact on their academic performance. Under this assumption, we constructed our machine learning model to predict student achievement based on these factors. Our findings show that the higher the poverty and unemployment rates in a students’ geographic region, the lower their test scores will be. Conversely, we found that the higher the income in a student’s household, the higher their test scores will be. 

What we can infer from this data is that a student’s socioeconomic status and access to resources plays a much more important role in their educational outcomes than the amount of funding a state receives for schools, or the amount of money a state spends on instruction. This information is vital for policy makers and stakeholders who have influence over the availability of funding and resources for our schools. These findings should be used to help make more informed decisions about how we view education in the United States in order to effectively promote student achievement.

## References
* [NAEP Website](https://nces.ed.gov/nationsreportcard/about/)
* [US Education Department](https://eddataexpress.ed.gov/)
* [US Census Bureau](https://data.census.gov/cedsci/)
* [US Bureau of Labor Statistics](https://www.bls.gov/)
