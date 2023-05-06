# Diabetes_predication_system
Symptoms of Diabetes
• Frequent Urination 
• Increased thirst 
• Tired/Sleepiness
• Weight loss 
• Blurred vision 
• Mood swings 
• Confusion and difficulty concentrating 
• frequent infections


Dataset: Here PIMA Indian diabetes data set is considered. The data set is taken from UCI machine learning repository. The data set consists of 9 attributes: number of times pregnant, plasma glucose concentration, diastolic blood pressure, triceps skin folds thickness, serum insulin, body mass index, pedigree type, age, and class. Here, the class label is binary classification. It has two values
•	Tested positive (1) which means diabetic
•	Tested negative (0) which says nondiabetic
	Data set
•	 https://www.kaggle.com/datasets/mathchi/diabetes-data-setiabetes | Kaggle 
Dataset Description:
•	Pregnancies: Number of times pregnant
•	Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
•	Blood Pressure: Diastolic blood pressure (mm Hg)
•	Skin Thickness: Triceps skin fold thickness (mm)
•	Insulin: 2-Hour serum insulin (mu U/ml)
•	BMI: Body mass index (weight in kg/(height in m)^2)
•	DiabetesPedigreeFunction: Diabetes pedigree function
•	Age: Age (years)
•	Outcome: Class variable (0 or 1)


Preprocessing: It involves cleaning and transforming the data to make it suitable for analysis. Here are some preprocessing techniques commonly used in movie recommendation systems:
•	Data cleaning: All the information used in our example should be only positive and if it is in negative we can say it has extra noise in it and we need to clean the data. Ex: age and pregnancy can not be negative.
•	Data integration: Here we have two different dataset from two sources that we can integrate in this stage with using table join operation so it become lossless conversion.
•	Data Reduction: Data reduction is reduce the data at some point but in our example we can not reduce it to any abstract level that will loss all the information that are related.
•	Data transformation: Check if the structure of the data is proper or not and if not then we make a proper structure..
These preprocessing techniques help to ensure that the data is clean, normalized, and transformed in a way that enables accurate analysis and prediction of user preferences for movie recommendations.

Data Mining Techniques: Association rule mining, clustering, and classification are all data mining techniques that can be applied to movie recommendation systems. Here is a brief overview of how each of these techniques can be used:

Classification:
	 It is used in supervised learning technique and we have data that is supervised and labelled with 0 and 1 so we can use classification algorithm.
	This will divide all the data in two or more layer and assign some value to it. It will return result as per the part the value lies.
Here in our example we will train model to divide in two parts one is true and other is false. And when new data comes if it lies in true part we can say person have diabetes and vice-versa.


Methodology:
In this section we shall learn about the various classifiers used in machine learning to predict diabetes. The different methods used are defined below. 

k-Nearest Neighbours:
In this we can plot data points in chart(graph) now after applying knn algo this will divide in parts in our case it is two it is either 1 or 0, now for prediction when we will plot new data point we will check which part is nearest from that datapoint and then, we will include that data point in that part.

Logistic Regression:
 Logistic regression can derive confidence level (about its prediction).
Logistic regression estimates the probability of an event occurring, such as patient have diabetis or not, based on a given dataset of independent variables. Since the outcome is a probability, the dependent variable is bounded between 0 and 1.

Decision Tree:
This classifier creates a decision tree based on which, it assigns the class values to each data point
The Decision Tree algorithm is a machine learning algorithm used for classification and regression tasks. It builds a tree-like model of decisions and their possible consequences, based on a set of training data. In our examples we used some attributes and classes yes or no based.


Continuing from the previous decision tree, if a patient has had more than six pregnancies, the next decision is based on their blood pressure, with patients who have a blood pressure of 70 or lower going down the right branch and those with higher blood pressure going down the left branch. If a patient has a blood pressure of 70 or lower, they are classified as not having diabetes (represented by "No" at the leaf node). If a patient has higher blood pressure, the next decision is based on their age, with patients who are 35 years or younger going down the right branch and those who are older than 35 years going down the left branch. If a patient is 35 years or younger, they are classified as not having diabetes (represented by "No" at the leaf node), while if they are older than 35 years, the final decision is based on their glucose level, with patients who have a glucose level of 154 or higher going down the left branch and those with lower glucose levels going down the right branch. If a patient has a glucose level of 154 or higher, they are classified as having diabetes (represented by "Yes" at the leaf node), while if they have lower glucose levels they are classified as not having diabetes (represented by "No" at the leaf node).

Again, this is just an example of a decision tree for diabetes prediction and the actual tree used in practice may have different attributes and cutoff values. The decision tree can be trained on a dataset of patients with known diabetes status and their medical attributes, and then used to predict the diabetes status of new patients based on their attributes. The accuracy of the decision tree can be evaluated using a separate test dataset, and the tree can be optimized using techniques such as pruning and hyperparameter tuning. 


