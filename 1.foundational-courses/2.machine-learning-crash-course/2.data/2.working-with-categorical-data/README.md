# 🏷️ Working with Categorical Data

Categorical data represents types or categories—things like colors, names, or device types. These values aren’t numeric by nature, but we still need to turn them into numbers so machine learning models can use them.

---

## 🔍 What is Categorical Data?

### 🟨 **Categorical Data**

Data that belongs to a group or label, not a measurable quantity.  
Example: "red", "blue", "green", or "apple", "banana", "grape".

### 🔢 **Numbers Can Also Be Categorical**

Just because something is a number doesn’t mean it’s numerical.  
Example: ZIP codes or product IDs—these are categories, not quantities.

---

## 🧠 Encoding Categorical Data

### 🔁 **Encoding**

The process of turning categories into numbers that models can understand.

### 📘 **Vocabulary**

A list of all possible categories (values) in a feature.

### 🔢 **Index Numbers**

Assigning a unique number to each category in the vocabulary.

### 🔲 **One-Hot Encoding**

Represent each category as a vector with one `1` and the rest `0`s.  
Example:  
"red", "green", "blue" → `[1,0,0]`, `[0,1,0]`, `[0,0,1]`

### 🌐 **Sparse Representation**

Storing only the non-zero parts of one-hot encoded vectors to save space.

### 🌱 **Sparse Feature**

A feature where most values are zero (like in one-hot encoding of large vocabularies).

---

## 📏 Advanced Encoding Methods

### ⚡ **Hashing (Feature Hashing)**

Use a hash function to map categories to numbers, reducing memory use. Useful for high-cardinality features.

### 📊 **Mean Encoding**

Replace each category with the average value of the target variable for that category.

---

## 🚩 Handling Issues with Categorical Data

### 🚨 **Outliers in Categorical Data**

Rare or unusual categories can disrupt training if not handled well.

### 🧱 **Encoding High-Dimensional Categorical Features**

Large vocabularies can cause models to slow down or overfit. Use hashing or embeddings.

### 🔢 **Discrete Feature**

A feature with a countable number of categories.

---

## ⚙️ Feature Crosses

### 🔀 **Feature Cross**

Combining two categorical features into one to capture relationships.  
Example: "user type" × "device" might help model behavior more precisely.

---

## 🧪 Additional Concepts

### 👨‍⚖️ **Human Raters**

People who label data. Their labels can be subjective.

### 🤖 **Machine Raters**

Automated systems that assign labels (e.g., spam detectors).

### ⚖️ **Inter-Rater Agreement**

How much different raters agree on a label. Low agreement can mean noisy data.

### 🌐 **High Dimensionality**

Too many categories or features can slow down training or cause overfitting.

---

## 🤖 In Neural Networks

Neural networks often use **embeddings** instead of one-hot encoding—dense vectors that represent categories more compactly and meaningfully.

---

Working with categorical data requires careful encoding and awareness of feature size and quality. With the right preparation, categorical features can greatly improve model performance. 🚀
