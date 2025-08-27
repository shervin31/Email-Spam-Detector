# 📧 Email Spam Classification: Machine Learning for Smarter Inboxes  

## 📖 Project Overview  
This project addresses a **critical challenge in digital communication**: identifying and filtering out spam emails.  
Using a real-world dataset of emails, we developed a machine learning pipeline to classify messages as **spam** (unwanted) or **ham** (legitimate).  

The goal is to build a **robust, data-driven spam detection system** that improves productivity, strengthens cybersecurity, and reduces the costs of dealing with phishing attempts.  

---

## 🎯 Business Objective  
Unsolicited spam emails flood inboxes every day, wasting time and increasing exposure to phishing and fraud.  
This project aims to:  
- **Enhance Productivity** → Reduce the clutter of irrelevant messages.  
- **Improve Security** → Catch potentially harmful content before it reaches users.  
- **Cut IT Costs** → Lower the resources spent managing spam.  
- **Provide Business Insights** → Understand spam patterns for better filtering strategies.  

---

## 📊 Dataset  
We use a **labeled email dataset** containing thousands of messages classified as spam or ham.  

- **Features**: Text content, email length, presence of HTML, and frequency of suspicious keywords.  
- **Target Variable**: `spam` (1 = spam, 0 = ham).  

---

## 🛠️ Technical Approach  

The project follows a full **CRISP-DM lifecycle**:  

### 🔍 Data Preprocessing & EDA  
- Cleaned missing values and standardized text.  
- Explored spam vs ham distributions.  
- Identified key differences: spam tends to be **longer**, **HTML-heavy**, and uses words like *“free,” “winner,” “urgent.”*  

### ⚙️ Feature Engineering  
- Extracted numerical features: email length, word counts, HTML tags.  
- Created **keyword-based indicators** (e.g., “cash,” “private,” “drug”).  
- Encoded categorical variables for modeling.  

### 🤖 Model Benchmarking  
- **Baseline Zero Predictor**: 74.5% accuracy, but failed on recall (0%).  
- **Logistic Regression**: Improved performance but initially low recall.  
- **Feature-Enhanced Logistic Regression**:  
  - Validation Accuracy: **88.1%** ✅  
  - Balanced across **precision, recall, and F1-score**.  

### 📈 Model Evaluation  
- Metrics: Accuracy, Precision, Recall, F1-Score, False Positive Rate (FPR).  
- ROC Curve & AUC used to visualize model separability.  
- Final model demonstrated strong **generalization** and **low false positives**.  

---

### 🔍 Critical Insights  
- **HTML-heavy emails** are much more likely to be spam.  
- Specific **keywords** are strong spam indicators.  
- **Length distributions** differ: spam tends to be longer and more variable.  

---

## 💡 Data-Driven Recommendations  
1. **Deploy the Model** → Integrate into corporate email systems for automated spam detection.  
2. **Monitor & Update** → Spam patterns evolve, so retraining with fresh data is key.  
3. **Security Policy Alignment** → Use the model alongside phishing filters and employee awareness training.  
4. **Balance Precision & Recall** → Tailor thresholds depending on whether **false positives** (legit emails flagged) or **false negatives** (missed spam) are more costly to the business.  

---

## 📁 Repository Structure  

