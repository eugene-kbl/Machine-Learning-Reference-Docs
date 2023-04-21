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
- Modeling
	- Data Split
	- Model Selection
	- Model Tuning
	- Model Comparison
- Evaluation
	- Evaluation Metrics for Classification models
	- Evaluation Metrics for Regression models
- Experiment/Test

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

## 4. Modeling

### 4.1 Data Split
- training (.7/.8) and testing (.3/.2) sets 
- training (.7/.8), validation (.1/.15), and testing (.1/.15) sets

### 4.2 Model Selection
- Based on data insight gathered up until now and the problem defined, decide on applicable models to implement.
- Typically, for Structured data Random Forest, XGBoost, and CatBoost work best, whereas for Unstructured data Deep Learning and Trasfer Learning work best.

### 4.3 Model Tuning
- TODO
- TODO

### 4.3 Model Comparison
- TODO
- TODO

## 5. Evaluation
Once reseach question was formulated, data analyzed, and model(s) selected, it is important to decide 'what defined a successful model's outcome'.
There are different evaluation metrics available for classification and regression models, and thus definition of success could mean achieving an evaluation metrics result being equal or greater for classification (say, 95% for accuracy) or lower for regression (say, Mean Absolute Error).  

### 5.1 Evaluation Metrics for Classification models
There are many metrics available for classification type models to consider, such as Accuracy, Recall, Precision, etc..
### 5.2 Evaluation Metrics for Regression models
There are many metrics available for regression type models to consider, such as MAE, RMSE, etc..

## 6. Experiment/Test
- TODO
- TODO
