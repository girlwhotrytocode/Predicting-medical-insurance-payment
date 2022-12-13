# IMSE-586_Team-2

This project is to assess the effectiveness of penalized linear regression, which has the same level of transparency and interpretability as standard regression, in estimating medical insurance payments with non-cost inputs. 

Background:  

Humans are vulnerable to various types of risk, danger, and uncertainty such as physical death and illness always present in the world (Kaushik et al., 2022). Following the pandemic, it is clear that a medical emergency can attack anybody, at any moment, and have a financial impact on the individual. Medical insurance policies are made to minimize the expense of risk factors for these sudden occurrences. There are numerous cases where insurance costs have grown abnormally in recent years. The expense of healthcare in the US today exceeds 17% of the GDP and it keeps rising (Morid et al., 2017). Health insurance costs are influenced by a variety of factors. Hence, accurate predictability and estimation of the appropriate cost of health insurance are critical to beneficiaries. 

Ordinary least squares (OLS) estimation of projected economic and clinical outcomes for risk adjustment reasons is still a mainstay of predicting medical insurance payments. The emerging literature investigates possible machine learning applications to predict medical insurance costs (Duncan et al., 1996). Various high-performance machine learning approaches are used in this research to introduce models with high predictive value. However, the reason for the slow adoption of advanced machine learning techniques in practice is that only a partial explanation of the results is feasible, requiring sophisticated interpretation by an expert analyst (Kan et al., 2019). Penalized linear regression models, on the other hand, could be simply used and interpreted even in circumstances when computational power is restricted. Therefore, the purpose of this study is to assess the effectiveness of penalized linear regression, which has the same level of transparency and interpretability as standard regression, in estimating medical insurance payments with non-cost inputs. 



Research Question:

- Can a high-performing linear regression model be built with only non-cost inputs?
- Which input feature is the most significant predictor in determining medical insurance payment?
- Between standard and penalized linear regression, which model best predicts future medical insurance payment? 



Data Set: 

The raw dataset was collected by Acme Insurance company  which was founded more than ten years ago and proudly experienced significant growth. Acme insurance company delivers superior customer service to the public by providing high-quality durable medical equipment to enhance the health and general wellness of their present and prospective customers. The data to be used in this project is an open dataset supplied to the public by Acme company, which contains demographic, physical health information, and medical insurance payment of the beneficiaries. The dataset comprises 7 columns of features and 1338 rows of customers. The medical insurance costs are provided against the insured's age, gender (female, male),  Body mass index (providing an understanding of the body, weights that are relatively high or low relative to height, objective index of body weight (kg/m^2) using the ratio of height to weight, ideally 18.5 to 24.9), number of children covered by health insurance, smoker (Yes, No), and the beneficiary's residential region in the US (northeast, southeast, southwest, northwest). The attributes are either numerical or category variables.

Age: age of primary beneficiary
Sex: insurance contractor gender [female, male]
BMI: Body mass index, providing an understanding of the body, weights that are relatively high or low relative to height, objective index of body weight (kg/m^2) using the ratio of height to weight, ideally 18.5 to 24.9
Children: number of children covered by health insurance/number of dependents
Smoker: whether the customer smokes or not [Yes, No]
Region: the beneficiary's residential area in the US [northeast, southeast, southwest, northwest]
Charges: individual medical costs billed by health insurance 

Link for the medical insurance payment dataset: https://www.kaggle.com/datasets/harshsingh2209/medical-insurance-payout



Methods: 
Python and R programming languages will be used in this project for the development and training of linear regression models for the prediction of medical insurance payment. The required libraries and packages that will be imported, followed by preprocessing of the medical insurance payment dataset and exploratory data analysis. The statistical summary of the dataset will be examined after checking the data type and null values in each column. The statistical summary includes the count, mean, standard deviation, and other statistics relevant to the dataset's columns. The relationship between each independent variable and the dependent variable, medical insurance payment, and the ANOVA test is also used to validate the features that have a high effect on the target. For the research question 'which input feature is the most significant feature in determining medical insurance payment?', the ANOVA test performed in exploratory analysis and the summary of the linear regression model will be used to determine whether there are significant differences in medical insurance payment in each independent variable and which variables best predict the model.

Then, the raw dataset will be applied to the standard and penalized linear regression models and the performance is analyzed. We will divide the training and testing datasets into 75% and 25%, respectively, and then use the training data to develop two linear regression models. In the case of penalized linear regression, parameter tuning will be performed. After testing the trained model with the test dataset, the two models' performance will be compared with evaluation metrics. Evaluation metrics will include accuracy, R-squared, adjusted R-squared, RMSE, MAPE, and PR. The performance indicators described in the evaluation metrics will be used to determine whether or not the linear regression models are practical and to reach a conclusion on the research question 'Can a high-performing linear regression model be created using just non-cost inputs?'. Furthermore, for the research question 'between standard and penalized linear regression, which model best predicts future medical insurance payment?', we will evaluate the effectiveness of penalized linear regression models in medical insurance payment after comparing the performance of the two models using the evaluation metrics we created.


