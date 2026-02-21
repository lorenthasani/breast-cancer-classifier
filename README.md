# 🧬 Breast Cancer Classification using Logistic Regression

This project implements a **Logistic Regression classifier** to predict whether a breast tumor is **benign** or **malignant** using the Wisconsin Breast Cancer dataset.

The goal of this project is to demonstrate a simple yet effective machine learning pipeline including:

- Data preprocessing  
- Handling missing values  
- Training a Logistic Regression model  
- Evaluating model performance  

---

# 📊 Dataset Information

Dataset used:  
**Wisconsin Breast Cancer Database (January 8, 1991)**  
Source: University of Wisconsin Hospitals, Madison  

Official Dataset Link:  
https://archive.ics.uci.edu/dataset/15/breast+cancer+wisconsin+original  

---

## 📌 Citation Request

This breast cancer database was obtained from:

Dr. William H. Wolberg  
University of Wisconsin Hospitals  
Madison, Wisconsin, USA  

Donor: Olvi Mangasarian  
Received by David W. Aha  
Date: 15 July 1992  

If you publish results using this database, please acknowledge this information and cite one or more of the following:

1. O. L. Mangasarian and W. H. Wolberg:  
   *"Cancer diagnosis via linear programming"*, SIAM News, Volume 23, Number 5, September 1990.

2. William H. Wolberg and O. L. Mangasarian:  
   *"Multisurface method of pattern separation for medical diagnosis applied to breast cytology"*,  
   Proceedings of the National Academy of Sciences, U.S.A., Volume 87, December 1990.

3. O. L. Mangasarian, R. Setiono, and W.H. Wolberg:  
   *"Pattern recognition via linear programming: Theory and application to medical diagnosis"*,  
   in *Large-scale numerical optimization*, SIAM Publications, 1990.

4. K. P. Bennett & O. L. Mangasarian:  
   *"Robust linear programming discrimination of two linearly inseparable sets"*,  
   Optimization Methods and Software 1, 1992.

---

# 📈 Dataset Overview

- **Number of Instances:** 699  
- **Number of Attributes:** 10 features + 1 class attribute  
- **Missing Values:** 16 instances contain a missing value denoted by "?"  
- **Class Distribution:**
  - Benign: 458 (65.5%)  
  - Malignant: 241 (34.5%)

---

## 🧾 Attributes

| # | Attribute | Domain |
|---|-----------|--------|
| 1 | Sample Code Number | ID |
| 2 | Clump Thickness | 1 – 10 |
| 3 | Uniformity of Cell Size | 1 – 10 |
| 4 | Uniformity of Cell Shape | 1 – 10 |
| 5 | Marginal Adhesion | 1 – 10 |
| 6 | Single Epithelial Cell Size | 1 – 10 |
| 7 | Bare Nuclei | 1 – 10 |
| 8 | Bland Chromatin | 1 – 10 |
| 9 | Normal Nucleoli | 1 – 10 |
| 10 | Mitoses | 1 – 10 |
| 11 | Class | 2 = Benign, 4 = Malignant |

---

# 🔄 Dataset Conversion (.data ➜ .csv)

The dataset provided by UCI was originally in `.data` format, which is a plain text file with comma-separated values and no headers.

To convert it into a `.csv` file:

1. Opened the `.data` file.
2. Added proper column names manually.
3. Saved the file as `breast_cancer.csv`.

Example of column headers added:

```
SampleCodeNumber, ClumpThickness, UniformityOfCellSize, 
UniformityOfCellShape, MarginalAdhesion, 
SingleEpithelialCellSize, BareNuclei, BlandChromatin, 
NormalNucleoli, Mitoses, Class
```

---

# ⚙️ Machine Learning Model

**Algorithm used:** Logistic Regression

Steps performed:

1. Data Cleaning  
   - Removed or handled missing values  
   - Converted data types to numeric  

2. Feature Selection  
   - Dropped the ID column (Sample Code Number)  

3. Train-Test Split  

4. Model Training using Logistic Regression  

5. Model Evaluation  
   - Accuracy score  
   - Confusion matrix  

---

# 📚 Past Research Usage

Earlier studies using this dataset achieved:

- 93.5% accuracy (two hyperplanes)  
- 95.9% accuracy (three hyperplanes)  
- 93.7% accuracy using 1-Nearest Neighbor (Zhang, 1992)  

---

# 🚀 How to Run

```bash
git clone https://github.com/lorenthasani/breast-cancer-classifier.git
cd breast-cancer-classifier
pip install -r requirements.txt
python main.py
```

---

# 📌 Project Purpose

This project was created for educational purposes to practice:

- Data preprocessing  
- Logistic Regression  
- Medical dataset classification  
- Model evaluation  

---

### 👨‍💻 Author
Lorent Hasani  
Computer Science Student
