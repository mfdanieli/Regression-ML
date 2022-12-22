# Regression-ML
 
![Banner](2.png)

## Predict ice-cream sales according to the weather

### 1. Project overview
 
- *What is the goal?* 
Predict ice-cream sales.
 
- *How will this question be investigated?* Train and test a linear regression model to associate temperature and ice-cream revenue, using the [Ice Cream Revenue Prediction
 Database](https://www.kaggle.com/tariquepce/ice-cream-revenue-prediction).

- *Why is this subjetc important?* 

  1. **69,3 billion dollars** is the estimated value of the ice cream market in 2022 [(Source)](https://www.finedininglovers.com/article/10-numbers-behind-ice-cream).

  2. Waste of materia-prima is a huge problem for the enviroment and for business. One way to avoid this issue is to estimate product sales.
     > It takes nearly 2000 L of water to produce 1 kg of ice cream [(Source)](https://healabel.com/i-ingredients/ice-cream).

  3. There is a correlation between the temperature and ice cream sales, according to [The Oxford Review](https://oxford-review.com/what-is-a-correlation/#:~:text=As%20temperatures%20rise%20ice%20cream,occur%20as%20the%20temperature%20rises.).

- *Hypothesis:* Ice-cream revenue can be predicted through temperature data, reducing waste of material.

 - *Data Science skills and tools:* data exploration, wrangling, and visualization, machine learning (libraries pandas, numpy, matplotlib, seaborn, and sklearn), and deployment (libraries BeautifulSoup and telebot).


### 2. Solution strategy 
- Import database.
- Data wrangling (in order to assure quality and useful data):
    - check missing values and data types.
- Data exploration and visualization (useful to identify which health characteristics have the greatest impact on the development of diabetes):
    - check data distribution, statitical metrics, correlations.
    - summarize main characteristics of the data, gain better understanding of relashionships and extract important variables.
- Machine learning model training and testing: linear regression model.
- Interpret model.
- Evaluate model performance and its implications.
- Acquire real-time temperature and predictive sales for the day through the telegram app.

### 3. Highligths of the results

- *Data analysis*   
    - Mean revenue is R$ 521.57, while average temperature of the dataset is 22.2°C (which is a typical day in São Paulo, for example).
    - The minimal registered temperature was 0°C, when the revenue was R$ 10.
    - Maximum temperature was 45°C, and R$ 1000 was the income.
- *Model performance and interpretation*
    - Average error of the model is R$ 19.
    - The model explains nearly 98% of the ice-cream revenue.
      > Demographic density, population's buying power and other aspects can affect sales. 
    - According to the adjusted coefficients, a 1°C increase is associated with an increase of R$ 21,41 in revenue.

### 4. Business implications
- The model can be useful in assisting a business to purchase the correct amount of raw material, avoiding waste at the end of the day.
- Product selection and marketing actions: during cold days, promotions or winter flavors can be offered.
       


***Take a look of how you can receive today's ice-cream revenue prediction in your Telegram:***


https://user-images.githubusercontent.com/97743505/158029433-bf4b9ffd-da6e-4859-abe5-335bb02c3958.mp4


