# Deep Learning Practical 2 – Adult Income Classification Using ANN

## 📌 Project Overview

This project focuses on implementing and evaluating an **Artificial Neural Network (ANN)** using Deep Learning techniques to predict whether an individual's annual income exceeds $50K based on demographic and employment-related attributes.

The project uses the Adult Income Dataset and explores different neural network configurations, activation functions, weight initialization methods, and loss functions to understand their impact on classification performance.

The main objective is to build an effective Multi-Layer Perceptron (MLP) model and compare different experimental configurations using appropriate evaluation metrics.

## 🎯 Objectives

- Understand the fundamentals of Artificial Neural Networks (ANN).
- Perform data preprocessing and feature engineering.
- Build a Multi-Layer Perceptron (MLP) architecture.
- Experiment with different activation functions.
- Compare different weight initialization techniques.
- Evaluate different loss functions.
- Understand the importance of Batch Normalization.
- Compare model performance using classification metrics.
- Identify an effective ANN configuration.

## 📂 Dataset Information

**Dataset:** Adult Income Dataset

The dataset contains demographic, educational, and employment-related information.

- Original records: 48,842
- Total columns: 15
- Target variable: `income`
- Classification type: Binary Classification

### Important Features

| Feature | Description |
|---|---|
| age | Age of an individual |
| workclass | Employment sector |
| education | Education level |
| education.num | Numerical education level |
| marital.status | Marital status |
| occupation | Type of occupation |
| relationship | Relationship status |
| race | Race category |
| sex | Gender |
| capital.gain | Capital gain |
| capital.loss | Capital loss |
| hours.per.week | Weekly working hours |
| native.country | Country of origin |
| income | Target variable |

### Target Variable

The target variable contains two classes:

- `<=50K` – Income less than or equal to $50K.
- `>50K` – Income greater than $50K.

## 🛠️ Technologies & Libraries Used

- **Python** – Programming language
- **TensorFlow** – Deep Learning framework
- **Keras** – ANN model implementation
- **NumPy** – Numerical computations
- **Pandas** – Data manipulation and preprocessing
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Data preprocessing and model evaluation

## ⚙️ Project Workflow

### 1. Data Loading

- Load the Adult Income dataset using Pandas.
- Examine dataset dimensions and data types.
- Understand the features and target variable.

### 2. Data Preprocessing

- Standardize column names.
- Remove unnecessary whitespace.
- Identify missing values.
- Replace missing-value markers (`?`) with NaN.
- Remove rows containing missing values.
- Drop unnecessary columns.
- Prepare numerical and categorical features.
- Encode categorical variables.
- Scale numerical features using StandardScaler.
- Split the dataset into training and testing sets.

### 3. ANN Architecture – Baseline Model

Build a Multi-Layer Perceptron using Keras Sequential API.

**Architecture:**

- Input Layer
- Hidden Layer 1 – 128 neurons
- Hidden Layer 2 – 64 neurons
- Output Layer – 1 neuron with Sigmoid activation

**Configuration:**

- Activation Function: ReLU
- Weight Initializer: Glorot Uniform
- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Batch Size: 64

### 4. Activation Functions

Experiment with different activation functions and analyze their impact on ANN performance.

- ReLU
- Sigmoid
- Tanh
- Leaky ReLU

Compare their learning behavior and classification performance.

### 5. Weight Initialization Techniques

Evaluate different weight initialization methods:

- Glorot Uniform
- Glorot Normal
- He Uniform
- He Normal
- Zeros Initialization

Understand how weight initialization affects neural network training and convergence.

### 6. Loss Functions

Experiment with different loss functions:

- Binary Crossentropy
- Weighted Binary Crossentropy
- Mean Squared Error (MSE)
- Focal Loss

Class weighting is also used to address class imbalance and improve minority-class recognition.

### 7. Batch Normalization

Apply Batch Normalization to hidden layers and investigate its effect on:

- Training stability
- Convergence
- Model performance

### 8. Final Combined ANN Model

Build a final combined ANN architecture using:

- 128 and 64 hidden neurons
- ReLU activation
- He Normal initialization
- Batch Normalization
- Adam optimizer
- Binary Crossentropy loss
- Class weighting

The final model combines selected techniques to evaluate their overall effectiveness.

## 📊 Model Evaluation Metrics

The models are evaluated using the following metrics:

| Metric | Purpose |
|---|---|
| Accuracy | Overall correct predictions |
| Precision | Correct positive predictions |
| Recall | Ability to identify positive cases |
| F1-Score | Balance between precision and recall |
| ROC-AUC | Ability to distinguish between classes |
| Confusion Matrix | Comparison of actual and predicted classes |

The project also includes:

- Training and validation performance plots.
- Classification reports.
- Confusion matrix visualization.
- ROC curve comparison.
- Final model comparison table.

## 📈 Results and Comparison

Different ANN configurations are compared based on their test performance.

The final comparison includes:

- Baseline ANN
- Activation function experiments
- Weight initialization experiments
- Loss function experiments
- Batch Normalization experiments
- Final combined ANN

The notebook generates a model comparison table and ROC curves to help identify the most effective configuration.

**Note:** Actual performance may vary depending on the training configuration and execution environment.


## 📁 Project Structure

```text
Deep_Learning_PR2/
│
├── deep_Learn_PR2.ipynb
│   └── Complete Deep Learning implementation
│
├── adult.csv
│   └── Adult Income dataset
│
├── results_table.csv
│   └── Generated model comparison results
│
└── README.md
    └── Project documentation
```

*Note: `results_table.csv` is generated when the final notebook cells are executed.*

## 📚 Key Learning Outcomes

Through this practical, I explored:

- Fundamentals of Deep Learning and ANN.
- Multi-Layer Perceptron architecture.
- Forward propagation and model training.
- Activation functions and their applications.
- Weight initialization techniques.
- Loss functions and class imbalance.
- Batch Normalization.
- Model evaluation and performance comparison.
- ROC curves and confusion matrices.
- Hyperparameter experimentation.

## 👨‍💻 Author

**Mant Sherasiya**

- GitHub: [Mant-0957](https://github.com/Mant-0957)
- Project Repository: [Deep_Learning_PR2](https://github.com/Mant-0957/Deep_Learning_PR2)

