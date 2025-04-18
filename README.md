# Differentiated Thyroid Cancer Analysis

## About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on Differentiated Thyroid Cancer Recurrence from [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/915/differentiated+thyroid+cancer+recurrence). For detailed walkthrough, please view the source code in order from:

1. [Data Preparations](https://github.com/Nomtt/SC1015_MiniProject_ECDS8/blob/a17a532f13739210e216e0eb46531692fae59c41/dataPrepFor_EDA.ipynb)
3. [Data Visualization](https://github.com/Nomtt/SC1015_MiniProject_ECDS8/blob/23eb20cbfd53615f50a21e1fc88cb0e4a38094de/exploratoryDataAnalysis.ipynb)
4. [Data Splitting](https://github.com/Nomtt/SC1015_MiniProject_ECDS8/blob/1d0634fbbfdcc476c732e25901de144b5f78c948/dataPrepFor_ML.ipynb)
5. [ML: Decision Tree Classification](https://github.com/Nomtt/SC1015_MiniProject_ECDS8/blob/94d41087e1d7ca026fdf5100471811b2efa495c5/decisionTreeRevised.ipynb)
6. [ML: Random Forest Classification and K-Clustering](https://github.com/Nomtt/SC1015_MiniProject_ECDS8/blob/ca7b7bbdf3751c02822794d084e452e18548cf7f/randomForestKClustering.ipynb) 
## Contributors
- Claire Chia Wan Ni (CLAI0011@e.ntu.edu.sg, @clairewanni ): 
  - Exploratory Data Analysis
  - Data Cleaning
  - Insights
  
- Narmandakh Nomt (nomt001@e.ntu.edu.sg, @nomtt ):
  - Machine Learning
  - Data Splitting
  - Recommendations

## Problem Definition

### Rationale
Differentiated Thyroid Cancer (DTC) is the most common thyroid cancer type which makes up over 90% of the cases. A key challenge is its unpredictability. Despite successful treatment, up to 30% of patients face recurrence. Current risk assessments rely on physician experience and generalized clinical guidelines, which may miss individual-specific factors that are affecting recurrence.

### Problem Statement
- Are we able to predict recurrence of Thyroid Cancer based on individuals’ physical attributes?
  - Which model would be the best to predict it?

## Models Used
- Decision Tree Classifier
- Random Forest Classifier
- K-means clustering

## Insights
- Initial treatment response is the most influential factor in likelihood of recurrence. If some cancer cells survive the initial treatment, they can eventually grow and lead to a recurrence. Therefore, patients who had severe responses should be given rigorous follow-ups.
- While more females were diagnosed overall, males experienced more severe complications and higher recurrence, suggesting that more rigorous follow-up protocols might be necessary for male patients.
- Recurrence risk increases with age. Greater monitoring and intervention should be prioritized for older individuals, even if their initial diagnosis appears mild.
- Although most patients were non-smokers, smokers consistently showed poorer recovery and higher recurrence rates, hence smoking as a lifestyle factor may warrant tighter follow-up treatments or additional counseling during and after treatment.
- Patients presenting with lymphatic spread (Adenopathy) or aggressive tumor types should be considered high-risk from the beginning, even before recurrence signs emerge.

## Conclusion
- We were able to develop a predictive machine learning model for the Cancer Recurrences using KClustering integrated with Random Forest Classifier with tuned hyperparameters trained on Dataset X3.
- Through iterative improvement from training 15 machine learning models, we successfully increased the accuracy of our model from as low as 66% at the beginning to 98.95% eventually.

## What did we learn from this project?
- Handling a medical dataset (Thyroid Cancer data) that includes a mix of numerical and complex categorical variables.
- Visualising and finding relationships between different variables
- Decision Tree Classification, Random Forest Classification (LEARNT), k-clustering (LEARNT)
- Observed how adding more features improves accuracy but risks overfitting with 4 different models with increasing feature complexity (X, X2, X3, X4)
- Understanding and usage of Accuracy and Hyperparameters
- New evaluation Metrics for KClustering, for instance, KMeans Inertia, Silhouette Score and Elbow Methods(WCSS) 

## Future Improvements
- Improve data balance
  -  While our model performed well, its predictive power could be further improved with more balanced datasets and additional clinical features like post-operative hormone levels.
- Explore time-based models
  - Since recurrence can happen years after treatment, future models could benefit from time-series analysis or longitudinal tracking to better capture recurrence timing.
- Embed model outputs into clinical settings
  - With minimal tuning, the model can serve as a real-time tool to help clinicians identify high-risk patients—such as older males with aggressive tumors—and customize their follow-up plans .

## References
- https://archive.ics.uci.edu/dataset/915/differentiated+thyroid+cancer+recurrence 
- https://www.geeksforgeeks.org/random-forest-regression-in-python/
- https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html
- https://www.analyticsvidhya.com/blog/2019/08/comprehensive-guide-k-means-clustering/
- https://www.kaggle.com/datasets/joebeachcapital/differentiated-thyroid-cancer-recurrence
- https://www.cancerresearchuk.org/about-cancer/thyroid-cancer/stages-types/types#:~:text=Differentiated%20thyroid%20cancer,follicular%20and%20oncocytic%20thyroid%20cancer.
- https://www.mayoclinic.org/diseases-conditions/thyroid-cancer/symptoms-causes/syc-20354161
- https://online.hbs.edu/blog/post/data-visualization-techniques
- https://mode.com/blog/violin-plot-examples
- https://thyca.org/newly-diagnosed/glossary/
- https://youtu.be/gSQsFIMcA8A?si=lCa8Ys1Dn4RYBJhQ
- https://youtu.be/gkXX4h3qYm4?si=Uc8ZzyC4fEvKwGNo
