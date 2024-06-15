# Cirrhosis: Project Overview
- Created a tool that determines what factors are affected by patients with Cirrhosis vs. those who do not.
  - Factors tested include ascites, spiders, edema, bilirubin, cholesterol, tryglicerides, and etc.
- Performed data cleaning in Python by omitting irrelevant attributes and removing duplicates/empty data.
- Extracted insights on the distribution of certain attributes through the creation of graphs using Pandas and Matplotlib.
- Performed data filtering and data manipulation to categorize and classify patients who use a certain drug to treat - Cirrhosis and those who have a specific symptom/condition.
  - e.g.: Classified those with Ascites, which is a condition in which fluid collects within your abdomen, into 1 (yes) or 0 (no) to determine if there's a correlation between Ascites and Cirrhosis.
- Created a model of the decision tree algorithm to predict the response for the data given.
  - Accuracy produced: 71.43%, indicating the model has good accuracy.
  
  # Resources Used 
  - Data used: https://www.kaggle.com/datasets/fedesoriano/cirrhosis-prediction-dataset 
  - Decision Tree Explanation: https://www.kdnuggets.com/2020/01/decision-tree-algorithm-explained.html
  
  # Data Cleaning
  The dataset I used may have had columns that were null, so I had to drop those columns. I made the following changes: 
  - Dropped columns that are null
  Since the dataset was from Kaggle, it was already clean and had all the relevant attributes, so no columns had to be added or deleted.
  
  # Exploratory Data Analysis
  I explored the data by displaying the distributions of certain attributes, such as cholesterol, bilirubin, albumin, copper, age, and other characteristics that may be impacted by the presence of Cirrhosis. Below are examples of the boxplots I created in Pandas. 
- Cholesterol
![Cholesterol](https://user-images.githubusercontent.com/51142303/212777606-e0aed0ba-3bb1-49df-982c-5e46cd9dc3cb.png)
  - In patients with cirrhosis, the levels of cholesterol are lower than those without.
- Bilirubin
![image](https://user-images.githubusercontent.com/51142303/212779322-2ca5524e-b12d-4bcf-b0e6-578797784a09.png)
  - Those with high levels of Bilirubin may have liver problems, such as Cirrhosis.
 
 I also used a heat map to visualize which variables are highly correlated (higher correlation - 1) vs. variables that are not.
 ![image](https://user-images.githubusercontent.com/51142303/212779420-90b2d7e0-3af7-4af1-8bf7-b3455aa641d5.png)

I graphed scatterplots to visualize the relationship between two variables. Below is an example of Tryglicerides vs. number of days with Cirrhosis: 
![image](https://user-images.githubusercontent.com/51142303/212779494-072aef62-08df-4cae-bd2c-7f0179b337c1.png)
  - There does not seem to be a strong correlation between these two variables.

# Conclusion
![image](https://github.com/acanna2013/CirrhosisProject/assets/51142303/f19ff582-90dd-4713-8f8c-028f1ecd401e)
\
Test set: Model resulted in ~71.43% accuracy. 

![image](https://github.com/acanna2013/CirrhosisProject/assets/51142303/09f8cf67-9e7f-499e-b468-7a04e931cfba)
\
Training set: Model resulted in ~82.43% accuracy.

![image](https://github.com/acanna2013/CirrhosisProject/assets/51142303/4f3957f7-ca51-452d-9149-9529b5d1b686)
\
Decision tree of the relationship between the relevant variables that may contribute to Cirrhosis. 



