# Student Scores Analysis: Statistics, Probability & Linear Algebra

A comprehensive Exploratory Data Analysis (EDA) notebook applying descriptive statistics, probability theory, distribution modeling, and linear algebra operations to a 5,000-student academic performance dataset.

---

## Dataset Overview

The dataset contains records for 5,000 students across 7 academic and demographic variables:

| Column Name | Type | Description |
| :--- | :--- | :--- |
| `Student_ID` | String | Unique student identifier (`STU_10000`–`STU_14999`) |
| `Age` | Integer | Student age (15–19)  |
| `Math_Score` | Numeric | Exam score in Mathematics |
| `Science_Score`| Numeric | Exam score in Science |
| `English_Score`| Numeric | Exam score in English  |
| `Hours_Studied`| Float | Total study hours  |
| `Pass_Fail` | Binary | Final outcome (1 = Pass, 0 = Fail)  |

---

## Key Analysis & Findings

### 1. Central Tendency & Dispersion
* **Math Score Tendency:** Mean of **51.34**, Median of **51.0**, and Mode of **44** .
* **Science Score Dispersion:** Standard deviation of **12.79**, variance of **163.56**, and overall range of **87** .

### 2. Probability & Contingency
* **Baseline Pass Rate:** Overall probability of passing $P(\text{Pass}) = \mathbf{58.74\%}$ .
* **Study Time Impact:** A contingency table evaluated the impact of studying over 5 hours :

| Pass / Fail | Hours Studied $\le$ 5 | Hours Studied > 5 | Total |
| :--- | :--- | :--- | :--- |
| **Fail (0)** | 923 | 1,140 | 2,063 |
| **Pass (1)** | 221 | 2,716 | 2,937 |
| **Total** | 1,144 | 3,856 | 5,000 |

* **Conditional Probability:** Studying $>5$ hours raises the probability of passing to $P(\text{Pass} \mid \text{Hours} > 5) = \mathbf{70.44\%}$].

### 3. Distribution & Normality
* **Histogram & Normal Curve:** Math scores follow a bell-shaped distribution centered around 51 .
* **Shape Metrics (Science Score):** Positively skewed (**0.292**) with positive (leptokurtic) kurtosis (**0.256**) .
* **Q-Q Plot:** English scores conform closely to a normal theoretical distribution .

### 4. Linear Algebra Operations
Vectors representing Math and Science scores for the first 5 students were evaluated :
* **Inner Product:** Dot product equals **11,054** .
* **Vector Norms:** $L_1$ Norm = **234.0**, $L_2$ Norm = **110.37** .
* **Vector Similarity:** Cosine similarity ($\cos \theta$) of **0.953**, yielding an angle of **17.63°** between Math and Science score vectors .

---

## Tech Stack

* **Language:** Python 3.11+[cite: 1]
* **Libraries:** `pandas`, `numpy`, `scipy`, `matplotlib` 

---

