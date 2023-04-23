# Machine-Learning-Framework
This repository is to be used as a guide for machine learning projects.
Below are the sections to be discussed:
- Research Question or Problem Definition
	- Supervised Learning
	- Unsupervised Learning
	- Reinforcement Learning
	- Transfer Learning
- Data 
	- Structured Data
	- Unstructured Data
	- Static Data
	- Streaming Data
	- Exploratory Data Analysis
- Features
- Evaluation
	- Evaluation Metrics for Classification models
	- Evaluation Metrics for Regression models
- Modeling
	- Data Split
	- Model Selection
	- Model Tuning
	- Model Comparison

## 1. Research Question or Problem Definition
- It is crucial to establish the problem or question that needs to be addressed before beginning the coding process.
- Understand the nature of the problem and determine the appropriate type of Machine Learning to be utilized.
- The four main types of machine learning are as follows:
	- Supervised Learning
	- Unsupervised Learning
	- Reinforcement Learning
	- Transfer Learning

### 1.1 Supervised Learning
In this type of machine learning, the algorithm is trained on labeled data, which means the data is already classified or labeled. The algorithm uses this labeled data to make predictions or classifications on new, unseen data.

### 1.2 Unsupervised Learning
In this type of machine learning, the algorithm is trained on unlabeled data, which means the data is not classified or labeled. The algorithm tries to identify patterns or relationships in the data without any prior knowledge.

### 1.3 Reinforcement Learning
In this type of machine learning, the algorithm learns by interacting with an environment. The algorithm receives rewards or punishments based on its actions and learns to take actions that maximize its rewards over time.

### 1.4 Transfer Learning
In this type of machine learning, knowledge gained from one task is leveraged to improve performance on another related task. A model that has been trained on a large and diverse dataset can be fine-tuned on a smaller dataset or a different task to improve its performance. Transfer Learning is particularly useful when the amount of data available for a specific task is limited or when training a model from scratch is computationally expensive. 

## 2. Data
- Structured/Unstructured
- Static/Streaming
- Exploratory Data Analysis

### 2.1 Structured Data
Structured data refers to data that is organized in a tabular format with rows and columns. This type of data is well-suited for traditional machine learning algorithms and can be easily processed and analyzed using statistical methods. 

### 2.2 Unstructured Data
Unstructured data refers to data that does not fit into a traditional tabular format and can include images, audio files, or natural language text. 

### 2.3 Static Data
Static data refers to data that is not expected to change over time, such as historical customer purchase data. 

### 2.4 Streaming Data
Streaming data refers to data that is generated continuously and can include sensor readings, social media posts, or financial transactions. 

### 2.5 Exploratory Data Analysis (EDA)
EDA refers to the process where the data is analyzed to understand its structure, identify patterns, and detect anomalies. EDA can also help to identify potential preprocessing steps that may be necessary before training a machine learning model.

## 3. Features
- Numeric
- Categorical
- Derived - Feature Engineering

## 4. Evaluation
Once research question was formulated, data analyzed, and model(s) selected, it is important to decide 'what defined a successful model's outcome'.
There are different evaluation metrics available for classification and regression models, and thus definition of success could mean achieving an evaluation metrics result being equal or greater for classification (say, 95% for accuracy) or lower for regression (say, Mean Absolute Error).  

### 4.1 Evaluation Metrics for Classification models
There are many metrics available for classification type models to consider, such as Accuracy, Recall, Precision, etc.
### 4.2 Evaluation Metrics for Regression models
There are many metrics available for regression type models to consider, such as MAE, RMSE, etc.

## 5. Modeling

### 5.1 Data Split
- training (.7/.8) and testing (.3/.2) sets 
- training (.7/.8), validation (.1/.15), and testing (.1/.15) sets

### 5.2 Model Selection
- Based on data insight gathered up until now and the problem defined, decide on applicable models to implement.
- Typically, for Structured data Random Forest, XGBoost, and CatBoost work best, whereas for Unstructured data Deep Learning and Transfer Learning work best.
- Assess initial performance of models, on the training set or a subset of it, with respect to selected performance metrics score and training time. 
- Consider the potential trade off of metrics score and training time.

### 5.3 Model Tuning
Once model's initial performance is acceptable based on the trade off, use validation set for tuning and/or training set (if data was split into two sets).
- Hyperparameters can be adjusted
- Hyperparameters are depended on selected models.
	- e.g., Adjusting number of trees or depth for Decision Tree or Random Forest algorithms.

### 5.4 Model Comparison
Model comparison is done on test set. A good model will yield similar results on the training, validation, and test sets. However, it is not uncommon to see a decline in performance (underfitting of overfitting).
- Underfitting
	- Training set has a significantly higher performance than a test set.
- Overfitting
	- Test set has a significantly higher performance than a training set.

Overfitting and Underfitting refer to a model not being able to generalize well. 
There are several reasons which this can happens, typically it is due to data leakage and data mismatch. 

Data leakage happens when some of test data leaks into training data and thus results in overfitting.
Data mismatch happens when testing data is different than training data, such as having different features in the sets. Therefore, it is important to train data on the same kind of data as test data.

To tackle over and under fitting, several approaches can be considered:
- Underfitting
	- Try different models 
	- Tune model hyperparameters
	- Reduce number of features
	- Other
- Overfitting
	- Collect more data
	- Try different models

Lastly, while comparing different models, it is important to compare the trade offs of performance metrics scope, training time, and testing time to select the model which not only helps to answer the research question well but also the time it took to produce the results (optimization for performance or prediction time trade offs).

