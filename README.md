# 🤖 Instagram Fake Account Classifier

A beginner-level machine learning project to classify Instagram accounts as **fake/spammer** or **genuine**, based on profile features like followers, following count, profile picture presence, and more.

---

## 📌 Project Description

This project uses supervised machine learning techniques to detect whether an Instagram account is fake or genuine. It includes **data preprocessing**, **exploratory data analysis (EDA)**, **model building (Logistic Regression & Decision Tree)**, and **final predictions** on a test dataset.

---

## 🗂️ Dataset Information

The dataset contains Instagram account metadata with the following files:

- `train.csv` – 576 labeled accounts (288 fake, 288 genuine)
- `test.csv` – 120 accounts for prediction

### Key Features:

| Feature                 | Description                                 |
|-------------------------|---------------------------------------------|
| profile pic             | 1 = has profile picture, 0 = no picture     |
| nums/length username    | Ratio of numeric characters in username     |
| fullname words          | Number of words in full name                |
| name==username          | 1 if name matches username, else 0          |
| description length      | Bio/description character length            |
| external URL            | 1 if URL exists in bio                      |
| private                 | 1 = private account, 0 = public             |
| #followers              | Number of followers                         |
| #follows                | Number of accounts followed                 |
| fake (target)           | 1 = fake account, 0 = genuine               |

---

## 🧪 Models Used

| Model               | Accuracy |
|---------------------|----------|
| Logistic Regression | 86.2%    |
| Decision Tree       | 87.1% ✅ |

---

## 📊 Exploratory Data Analysis Highlights

- Fake accounts **rarely have profile pictures**
- Fake accounts are **mostly public**
- Fake accounts tend to **follow more people** and **have fewer followers**
- Created visualizations like:
  - Heatmaps
  - Boxplots
  - Countplots
  - Scatter matrix
  - Feature importance graph

---

## 🔧 Tools & Technologies

- **Language**: Python  
- **Environment**: Google Colab  
- **Libraries**:
  - `pandas` & `numpy` – data manipulation
  - `matplotlib` & `seaborn` – data visualization
  - `scikit-learn` – machine learning models and evaluation

---

## 📁 Folder Structure

```bash
📂 Instagram-Fake-Account-Classifier/
│
├── 📄 train.csv
├── 📄 test.csv
├── 📄 Instagram_Fake_Account_Classifier.ipynb
├── 📄 README.md

