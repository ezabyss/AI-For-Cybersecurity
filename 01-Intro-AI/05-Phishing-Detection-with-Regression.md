# 📧 AI for Cybersecurity: Spam Detection using Regression & Decision Trees

---

# 📌 1. Big Picture

👉 Goal:
Use **Machine Learning algorithms** to detect:
- Spam 🚨  
- Ham (normal) ✅  

👉 Algorithms covered:
1. Linear Regression  
2. Logistic Regression  
3. Decision Tree  

---

# 🧠 2. Core Understanding 

- Linear Regression → Predicts numbers (not ideal for spam)
- Logistic Regression → Predicts probability (good for classification)
- Decision Tree → Rule-based decisions (very effective)

---

# ⚔️ 3. Algorithm Comparison (IMPORTANT)

| Algorithm | Type | Best For | Performance |
|----------|------|---------|------------|
| Linear Regression | Continuous | Numeric prediction | ❌ Poor for spam |
| Logistic Regression | Classification | Probability-based | ✅ Good |
| Decision Tree | Classification | Rule-based | 🔥 Best |

---

# 📊 4. Dataset Understanding

Each row = SMS message

| Message | Label |
|--------|------|
| "Win money now" | Spam |
| "Hey how are you" | Ham |

---

# 🔍 5. Feature Engineering

👉 Convert text → numbers

### Example:

| Feature | Value |
|--------|------|
| spam keyword frequency | 3 |
| normal word frequency | 1 |

---

# 🧪 6. Linear Regression (NOT IDEAL)

## 📌 Concept
- Creates a **straight line**
- Predicts continuous values

---

## ⚠️ Problem

👉 Spam detection = classification  
👉 Linear regression = continuous output  

❌ Result:
- Poor accuracy  
- Not suitable  

---

## ❗ Limitations
- Assumes features are independent  
- Not good for classification  
- Weak performance  

---

# 🧠 7. Logistic Regression (BETTER)

## 📌 Concept

👉 Predicts **probability (0 to 1)**

- Output:
  - 0 → Ham  
  - 1 → Spam  

---

## 🔁 Process

1. Apply **one-hot encoding**
2. Convert categorical → numerical
3. Train model
4. Test model

---

## 📦 Dataset

- 30 features  
- Generated using **one-hot encoding**

---

## ✅ Advantages
- Good for classification  
- Probabilistic output  
- More accurate than linear regression  

---

## ⚠️ Limitation
- Assumes features are **linearly independent**

---

# 🌳 8. Decision Tree (BEST IN THIS CASE)

## 📌 Concept

👉 Makes decisions like a flowchart

---

## 🧠 How It Works

Example:

IF "free" present → spam  
ELSE IF "hello" → not spam  

---

## 🔁 Process

1. Use same dataset (one-hot encoded)
2. Split into training/testing
3. Train decision tree
4. Test model

---

## ✅ Advantages

- High accuracy  
- Easy to understand  
- Works with small data  
- No need for heavy math  

---

## ⚠️ Limitation

- Sensitive to small data changes  
- Can overfit  

---

# 🧍 9. Real-World SOC Scenario

## 📩 Email:

> "Click here to claim your free reward"

---

## 🔍 Model Behavior

### Linear Regression ❌
- Gives numeric value → unclear decision

---

### Logistic Regression ✅
- Predicts probability:
  - 0.85 → Spam

---

### Decision Tree 🔥
- Checks rules:
  - "free" + "claim" → Spam

---

## 🚨 Final Action

- Block email  
- Alert SOC  
- Prevent attack  

---

# ⚙️ 10. ML Development Process (Applied)

## 🔁 Steps

1. Data Collection  
2. Feature Engineering  
3. Model Selection  
4. Training  
5. Testing  
6. Evaluation  

---

# 🔧 11. Key Techniques

## 🔹 One-Hot Encoding

👉 Converts categories → numbers

Example:

| Feature | Value |
|--------|------|
| has_link | 1 |
| has_attachment | 0 |

---

# 🎯 12. Memory Tricks

👉 Linear Regression = straight line → ❌ spam  

👉 Logistic Regression = probability → ✅ spam  

👉 Decision Tree = rules → 🔥 best  

---

👉 If problem = classification  
👉 Use Logistic or Decision Tree  

---

# 🧠 13. Final Understanding

- Linear Regression is simple but weak  
- Logistic Regression improves classification  
- Decision Tree is powerful and intuitive  

---

# 🎯 ONE-LINE SUMMARY

👉 **Decision Tree > Logistic Regression > Linear Regression for spam detection**

---

## ✍️ Notes By Abhishek (Ez Abyss)
