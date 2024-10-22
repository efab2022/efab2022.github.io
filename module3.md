# Module 3 - Machine Learning

Module 3 was about machine learning:
- supervised and unsupervised machine learning
	- linear models
	- tree-based models
	- ensemble models
	- boosted models
	- clustering model
	- dimensionality reduction models
	- hyperparameter tuning
- ML fundamentals
	- Linear Algebra
	- Statistics & Hypothesis Testing
	- Calculus
- Working with datasets
	- imbalanced datasets
	- larger-than-memory datasets
	- leveraging parallel computing
- modelling
	- model selection
	- model evaluation
- working with features
	- feature selection
	- feature engineering
- Libraries/Frameworks
    - scikit-learn
    - xgboost
    - lightgbm
    - catboost
- cloud deployment
	- google cloud platform
	- streamlit
	- flask
	- fastapi
	- docker


## Sprint 9 - Travel Insurance

**Project Requirements**: In this project we perform market segmentation and customer analysis. The goal is to train a model to identify potential customers for a travel insurance, based on historical data.

**Key Learnings**:
- supervised machine learning
- model selection
- feature selection
- feature engineering
- business perspective: selecting a metric to measure success
- model evaluation
- ensemble models: bagging, boosting, ...
- creating custom loss functions


**Reviewer's highlights**:

> Score: 87

> - awesome business analysis and business requirement setting
> - I liked your modelling flow - goal setting, EDA, data preprocessing, modelling, eval --> iterate
> - loved your code. Great abstractions, OOP practices and generally - exemplary code quality
> - great advanced ML techniques, like custom scoring functions

![insurance.png](img/insurance.png)




## Sprint 10 - Stroke Risk

**Project Requirements**: This project requires training a model to predict stroke risk and to deploy it with a simple web/mobile frontend, so users can enter their data and see a predicted score/risk.

**Key Learnings**:
- supervised machine learning, same as previous projects.
- model packaging and deployment
- creating a small cloud app using streamlit

![](img/stroke1.png)

![](img/stroke2.png)

You can still find the deployed app over here: https://ealmas-stroke-risk.hf.space/

Since it's on a free account, the first page load takes about a minute to spin up the service.


**Reviewer's highlights**:

> Score: 96

> - Extraordinary job. You nailed it from the EDA to the evaluation and deployment. All the comments that I have are really minor ones:
> - Try to think of modeling as iterative process, spend more time trying different techniques (for example different imputation techniques, different scalers, dealing with imbalances). Scikit-learn pipelines give you ability to actually test even different combinations of them
> - Do not forget code quality: type hints should be used for the outputs of the function as well. Some larger functions might require docstrings; some charts were lacking namings as well.
> 
> I will hope to see more works like this :)




## Sprint 11 - Loan Prediction

**Project Requirements**: The first dataset over 2 million rows, with abundant EDA, cleaning and preprocessing, and 4 objectives:
- predicting loan acceptance/rejection
- predicting load grade
- predicting loan subgrade
- predicting loan interest
- create a custom backend with flask 
- deploy the model to GCP google cloud platform

**Key Learnings**:
- larger-than-memory data wrangling, cleaning and model training using various techniques (dask and custom libraries)
- created custom wrapper for optuna to leverage multi-core computation
    - learned why linux is loved when it comes to data science.
- developed custom utils to cache and snapshot intermediate steps in processing to ensure only non cached steps are excuted.
    - this allowed to ensure that all steps of computation can be done end to end as well as to skip intermediate steps when needed.

![](img/optuna-multiprocessing2.png)
___

on multiprocessing:
![](img/optuna-multiprocessing.png)
___

on caching:
![](img/caching_utils.png)


**Reviewer's highlights**:

> Score: 94

> Awesome job! Your project was very insightful and I really liked how you presented it. Also, I have no doubt that you are extremely good developer. With the set of skills you already have and Data Science knowledge, you would be a perfect fit for ML engineer position :) 



## Sprint 12 - Home Credit

**Project Requirements**: this capstone project focuses on the end-to-end lifecycle:
- translating business requirements into data science tasks
- selecting evaluations metrics and goals
- EDA, data cleaning, statistical inferencial analysis, ...
- feature engineering and data preprocessing
- using machine learning to solve business problems
- deploying multiple machine learning models to cloud


**Key Learnings**:
- this project did not necessarily require new skills, but was a really good opportunity to practice and apply the skills already learned, and to apply them in a more structured and methodical way.
- Most of the learnings and the most fun part was around further improving the library to parallelize, and store, all models and their hyperparameters, so they can be retrieved and analyzed at a later stage.
    - expanding the underlying structure to support ensemble models, and to allow capturing hyperparameters for inner models.

![](img/credit_score1.png)
___

this project also had 3 confidential features that had a lot of predictive power, but were labelled poorly intentionally. Those 3 confidential features also had some small gaps and missing values. One of the core goals was to try different imputation strategies to fill in the blanks, and to try visualize how they spread and contribute to the final target label.

![](img/credit_score2.gif)
___

some of the work to enhance the custom optuna wrapper library:
![](img/optuna_3.png)



**Reviewer's highlights**:

> Score: 

> - Great work! Extensive analysis and solution. Everything performed well from the technical side, all steps were taken to train and deploy the solution.
- You are very confident presenting and have a good understanding of the solution. Good job on trying out multiple different techniques in basically every step of your analysis - much work was put in it!



# Module 4

Continue to ⏩ [Module 4 - Deep Learning](module4.md) to review the next set of projects.

