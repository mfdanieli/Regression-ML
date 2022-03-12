# Regression-ML
 
![Banner](imagem.png)

## Predict diabetes according to risk factors

### 1. Project overview
 
- *What is the goal?* 
Predict if a pacient has diabetes.
 
- *How will this question be investigated?* Train and test the KNN model to associate risk factors and diabetes, using the [Pima Indians Diabetes Database](https://www.kaggle.com/uciml/pima-indians-diabetes-database).

- *Why is this subjetc important?* 

  1. A [recent study](https://diabetesjournals.org/care/article/42/9/1609/36309/Understanding-the-Economic-Costs-of-Diabetes-and) estimates that undiagnosed diabetes can cost **$31.7 billion annually**.

  2. In India, close to **42%** of the people with diabetes **are not aware** of their disease status, according to [Claypool  et al. (2020](https://drc.bmj.com/content/8/1/e000965?utm_content=americas&utm_campaign=usage&utm_medium=cpc&utm_source=trendmd&tid=xRcC2XdbS3AruBxKod5PPqdgMH1tPvz6BDUBfpZxRBxbqeyVrGycvEwy6xcPsIS8dQipAA==)).

  3. Diabetes tests can cost up to $29 in India ([Patra, 2021](https://www.breathewellbeing.in/blog/list-of-diabetes-test-blood-glucose-level-normal-values-procedure-cost/)). These costs can add up, since these tests often are retaken before a final diagnosis.

- *Hypothesis:* Diabetes can be diagnosed based on risk factors trhough modeling, reducing costs of exams and increasing diabetes identification among the population.

 - *Data Science skills and tools:* data exploration, wrangling, and visualization, machine learning (libraries pandas, numpy, matplotlib, seaborn, and sklearn).


### 2. Solution strategy 
- Import database
- Data wrangling (in order to assure quality and useful data):
    - check missing values and data types 
- Data exploration and visualization (useful to identify which health characteristics have the greatest impact on the development of diabetes):
    - check data distribution, statitical metrics, correlations
    - summarize main characteristics of the data, gain better understanding of relashionships and extract important variables
- Standardize the variables: important to garantee proper scales
- Machine learning model training and testing: KNN model
- Select optimal *k* value through the elbow method
- Evaluate model performance and its implications

### 3. Highligths of the results

- *Data analysis*
    - 35% of the people in the dataset have diabetes.
    - The disease is mostly correlated with glucose levels, followed by BMI (Body Mass Index).
    - Women with more pregnanies are mostly like to have diabetes.
    - People with higher BMI and skin thickness have the tendecy to develop diabetes.
- *Model performance*
    - Model accuracy is 75%.
      > For comparison,  24% of participants in a recent [study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6640891/#:~:text=Twenty%2Dfour%20percent%20of%20participants,137.2%2C%20P%20%3C0.001) reported being misdiagnosed with another condition before being diagnosed with type 1 diabetes.    
    - false negatives are 8% in the test dataset.
      > In diagnosis prediction, it is important to minimize false negatives, even if false positives are increased. This means that is preferable a model that says a person has diabetes (and in reality it is not true), other than a model that misses real positive diagnoses. 

### 4. Business implications
- The model can be useful in assisting a doctor to investigate whether a person has diabetes and which is the best treatment in two ways:
    - It can help to decide if a simple blood glucose meter or a more sophisticated test (and therefore more expensive) would be necessary. 
    - Increase early detection and awareness.
      > People with diagnosed diabetes incur average medical expenditures of $16752 per year ([ADA, 2018](https://www.diabetes.org/about-us/statistics/cost-diabetes)). Medical care for prediabetes, on the other hand, costs $500 annually per person ([AMA, 2019](https://www.ama-assn.org/delivering-care/diabetes/how-prediabetes-exacts-43-billion-toll-us-economy#:~:text=On%20average%2C%20prediabetes%20costs%20%24500,person%20in%20medical%20costs%20only.)).
        
### 5. Conclusions
In 2030, it is expected that the global burden of diabetes will reach USD 825 billion, affecting mainly middle and low-income countries ([Williams et al., 2020](https://www.diabetesresearchclinicalpractice.com/article/S0168-8227(20)30138-8/fulltext)). Therefore, prevention and early diagnosis are imperative. 
The developed model showed reasonable accuracy to identify diabetes, based on health risk factors, and using a case study from India. The results indicate that test costs might be decreased, assisting doctors in diagnostics and treatments.  


### 6. Suggestions for further steps
- Select only those features with higher impact on developing diabetes:
    - This might reduce the number of exams (therefore, costs), since not all risk factors would be significant enough. Other classification machine learning techniques (e. g. decision trees) could be applied.
- Improve model accuracy using k-Fold Cross-Validation, for example.


***Take a look at an app that I build, where you can input your own data and check in real time the chance to develop diabetes:***


https://user-images.githubusercontent.com/97743505/158029433-bf4b9ffd-da6e-4859-abe5-335bb02c3958.mp4


