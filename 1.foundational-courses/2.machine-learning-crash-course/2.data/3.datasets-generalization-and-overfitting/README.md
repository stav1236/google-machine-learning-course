# 🧠 Datasets, Generalization, and Overfitting

This section introduces important concepts about datasets, how to prepare data for machine learning, and how to train models that generalize well without overfitting.

---

## 📁 Dataset Fundamentals

### 📦 **Dataset**

A collection of data examples used to train and evaluate ML models.

### 🧪 **Example**

One row in the dataset—includes features and (in supervised learning) a label.

### 🔣 **Feature**

An individual measurable property or input variable.

### 🏷️ **Label**

The target value the model is trying to predict.

---

## 🧠 Types of Data

- **Numerical data** – Numbers with magnitude (covered separately)
- **Categorical data** – Named groups or categories (covered separately)
- **Text / Human language** – Words, sentences, documents
- **Multimedia** – Images, videos, audio
- **Outputs from ML models** – Example: embedding vectors
- **Embedding vector** – A dense numeric representation of data, like words or categories

---

## 📊 Data Quality

### 🔢 **Quantity of Data**

More examples often help, but quality is critical.

### ✅ **Quality and Reliability**

Clean, correct, and consistent data leads to better models.

### ⚠️ **Complete vs. Incomplete Examples**

Missing features or labels can cause problems—use **value imputation** to fill gaps.

### ⚙️ **Value Imputation**

Replacing missing values with substitutes (e.g., mean, median, or a placeholder).

---

## 🧼 Data Preprocessing

### 📏 **Z-score Normalization**

Standardizes values by subtracting the mean and dividing by standard deviation.

### 🔄 **Transforming Data**

Includes normalization, encoding, scaling, and cleaning.

### ⚠️ **NaN Trap**

Models can silently break if missing values (`NaN`) are not handled.

### 🧽 **Scrubbing**

Cleaning up bad, noisy, or inconsistent data.

### 🔎 **Filter Examples Containing PII**

Remove personal identifiable information to protect user privacy.

---

## 📉 Dataset Balance

### ⚖️ **Class-Imbalanced Dataset**

When one class appears far more often than others.

- **Majority class** – The more common class
- **Minority class** – The less frequent class
- **Imbalanced datasets** – Lead to bias in predictions
- **Prediction bias** – Model prefers the dominant class

### 🛠️ Fixing Imbalance

- **Downsampling** – Reduce majority class samples
- **Upweighting** – Give more importance to minority class during training
- **Rebalance ratios** – Adjust how classes are treated
- **Baseline** – A simple prediction strategy used for comparison

---

## 📚 Label Types

### 🏷️ **Direct Label**

The real-world outcome you're interested in. Example: clicked = yes/no

### 🕵️‍♂️ **Proxy Label**

An indirect substitute when the true label isn't available. Example: time on page = engagement

---

## 👥 Data Sources

- **Human-generated data** – Created or labeled by people
- **Automatically-generated data** – Collected by systems or logs
- **Human raters** – People who label data manually
- **Machine raters** – Automated systems labeling data

### 📊 **Inter-rater Agreement**

How much different human raters agree on the label. Low agreement = noisy labels.

---

## 🧠 Generalization

### 🧩 **Generalization**

The ability of a model to perform well on new, unseen data.

### 🔄 **Generalization Curve**

Shows the difference between training and validation performance over time.

### ✅ Good Generalization Requires:

- **I.I.D.** – Examples are _independent and identically distributed_
- **Stationarity** – The data distribution doesn’t change over time
- **Matching partitions** – Training, validation, and test sets follow the same distribution
- **No data leakage** – No overlap between training and test/validation sets

---

## 📊 Dataset Splits

- **Training set** – Used to teach the model
- **Validation set** – Used to tune hyperparameters and detect overfitting
- **Test set** – Used to evaluate final model performance

### ✅ A good test/validation set should:

- Be **large enough** for statistically meaningful results
- Be **representative** of both the dataset and real-world data
- Contain **no duplicates** from the training set

---

## ⚠️ Overfitting & Underfitting

### 📈 **Overfitting**

Model memorizes training data but fails on new data.

### 📉 **Underfitting**

Model is too simple and can’t learn from the data.

### 📊 **Loss Curve**

Plots training and validation loss during training.  
If validation loss increases while training loss decreases → overfitting.

### 🧠 **Model Complexity**

More complex models can overfit if not regularized.

---

## 🔧 Controlling Overfitting

### 🧩 **Regularization**

Adds a penalty to reduce model complexity.

- **L1 regularization** – Makes some weights zero (feature selection)
- **L2 regularization** – Shrinks all weights slightly (smooths model)
- **Regularization rate (lambda)** – Controls the penalty strength
- **Loss and complexity** – Find a balance between accuracy and simplicity

### ⏱️ **Early Stopping**

Stop training when validation performance stops improving.

### ⚖️ **Finding Equilibrium**

Balance **learning rate** with **regularization rate** to avoid both overfitting and underfitting.

---

## ⚙️ Additional Terms

- **Mini-batch** – A small group of training examples used in one step of optimization
- **Batch** – Similar to mini-batch, but may be larger
- **Hyperparameter** – Settings you configure before training (e.g., learning rate, batch size)

---

A well-prepared dataset and a properly regularized model are essential to good ML results. Generalization is your goal—overfitting is the trap. ✅
