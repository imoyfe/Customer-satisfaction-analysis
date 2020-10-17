# Customer Satisfaction with Sentiment Analysis

#### This project is aimed to explore the level of satisfaction of our customers by analyzing different KPIs, scored from 0 to 5 being 0 the lowest level of satisfaction and 5 the highest:
* Expectations
* Lecturers
* Workload
* Methodology
* Comments (some text to process with NLP techniques)

#### some demographic data (both, numerical and categorical):
* Age
* Gender (M = man, F = woman)
* Job
* Experience (years of professional experience)
* Studies (level of studies: degree, master, PhD, professional)
* Income
* Country

#### and some characteristics to identify the product analyzed:
* Product (the label of the observation: A, B, C and D)
* Language (0 = EN, 1 = ES)

### Contents:
* 2 datasets (with synthetic generated data English and Spanish)
* 2 notebooks, one for analysis and another one for topic modelling classification
* some images to illustrate the insights

![Expectations by Countries](https://github.com/imoyfe/Customer-satisfaction-analysis/blob/master/images/expectations_by_countries.png)

![Expectations by Studies and Product](https://github.com/imoyfe/Customer-satisfaction-analysis/blob/master/images/expectations_by_studies.png)

01. Customers_Satisfaction_Analysis.ipynb
> In the first notebook we followed the first steps of a machine learning pipeline: Data cleaning and Explaoratory Data Analysis (EDA)
> We also used some NLP libraries for sentiment analysis of the customers' comments such as VADER (English) and SENTY (Spanish).

![Topic 1](https://github.com/imoyfe/Customer-satisfaction-analysis/blob/master/images/wordcloud.png)

02. Topic_modelling.ipynb
> In the second notebook used the TfIdf Vectorizer in order to obtain lists of the most frequent words and infer 3 main topics.
> We generated some wordclouds per each topic
> Finally, we applied a classification model (Multinomial NB) and according to the evaluation metrics of the model it resulted simply random.

![Model Metrics](https://github.com/imoyfe/Customer-satisfaction-analysis/blob/master/images/metrics.png)

Next steps should be considering FINE TUNING the model or even trying differnt classification models.
