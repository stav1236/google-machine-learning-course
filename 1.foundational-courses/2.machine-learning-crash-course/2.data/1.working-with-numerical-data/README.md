# 🔢 Working with Numerical Data

In machine learning, how we prepare and transform numbers matters. Good data makes better models. This section covers key ideas for analyzing and preparing numerical data for training.

---

## 📊 Data Types

### 🟦 **Numerical Data**

Data with measurable quantities (e.g., height, age, price).

### 🟨 **Categorical Data**

Data that represents categories or labels (e.g., "red", "male", "yes").

---

## 🛠️ Preparing and Transforming Data

### 📦 **Binning / Bucketing**

Group continuous values into ranges.  
Example: Age 0–18 → “child”, 19–60 → “adult”.

### ⚙️ **Feature Engineering**

Creating new useful features from existing ones.

### 📐 **Feature Vector**

A list of features that describes one data point. It's what the model actually uses.

### ♻️ **Normalization**

Make different features comparable by putting them on the same scale.

### 🧼 **Preprocessing**

All steps done to clean, transform, and prepare raw data before training.

---

## 📈 Understanding the Data

### 📊 **Visualize Your Data**

Use plots (e.g., histograms, scatter plots) to detect trends, gaps, or errors.

### 📉 **Statistically Evaluate Your Data**

Understand your data’s shape and spread using numbers.

- **Mean and Median**: Average vs. the middle value
- **Standard Deviation**: How spread out the numbers are

### 🚩 **Find Outliers**

Extreme values that don’t fit the pattern. Can affect training badly.

### ✂️ **Clipping**

Limit extreme values to a set range to reduce the impact of outliers.

---

## 📏 Scaling Methods

### 🔄 **Normalization (Rescaling)**

Shrink all values to a range like 0 to 1.

### 📊 **Linear Scaling**

Adjust values proportionally based on the min and max.

### ⚖️ **Z-Score Scaling**

Standardize based on mean and standard deviation.

### 📉 **Log Scaling**

Use logarithms to reduce the effect of large values.

---

## ⚠️ Common Pitfalls

### 🚫 **NaN Trap**

Missing or "Not a Number" values can silently break training if not handled.

### 🧽 **Scrubbing**

Cleaning bad, missing, or inconsistent data.

---

## 🔍 Label and Dataset Structure

### 🏷️ **Label**

The correct answer in supervised learning (e.g., “spam” or “not spam”).

### 📦 **Dataset**

A collection of examples, each with features (and sometimes labels).

---

## ✅ Good Feature Practices

- **Clearly Named**: Easy to understand and track
- **Checked Before Training**: Verified for correctness and consistency
- **Sensible**: Relevant to the task

---

## 🧪 Feature Engineering Techniques

### 🔢 **Polynomial Transforms**

Use powers of a feature (e.g., age²) to capture non-linear patterns.

### 🧬 **Synthetic Feature**

New feature created by combining or transforming others.

### 🔀 **Feature Cross**

Combine two features into one to capture interactions.  
Example: “day” × “location” to model traffic patterns.

---

Having clean, well-scaled, and meaningful numerical data is essential. Models can only learn well from data that makes sense. 💡
