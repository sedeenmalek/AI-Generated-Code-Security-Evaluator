# AI-Generated Code Security Evaluator 
An automated machine learning pipeline designed to evaluate the security posture of source code, detect potential vulnerabilities, and classify functions as **Secure (0)** or **Vulnerable (1)**[cite: 1].
---
##  Dataset Overview
The models were trained and evaluated on a unified, multi-source code dataset containing **5,133 source code functions**[cite: 1]:
* **Secure Functions (0):** 4,358[cite: 1]
* **Vulnerable Functions (1):** 775[cite: 1]
---
##  Evaluated Models & Results

Three distinct machine learning classifiers were implemented and benchmarked on a test split of **1,027 functions**[cite: 2, 4, 6]:

| Model | Overall Accuracy | Vulnerable Precision | Vulnerable Recall | Vulnerable F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **XGBoost (Best)** | **95%**[cite: 4] | **0.91**[cite: 4] | **0.72**[cite: 4] | **0.81**[cite: 4] |
| **Random Forest** | 94%[cite: 2] | 0.99[cite: 2] | 0.61[cite: 2] | 0.75[cite: 2] |
| **Logistic Regression** | 91%[cite: 6] | 0.66[cite: 6] | 0.75[cite: 6] | 0.71[cite: 6] |

### Key Findings
* **XGBoost** achieved the strongest overall performance and balance across precision and recall, making it the primary recommended model for vulnerability assessment[cite: 4].
* **Random Forest** demonstrated the highest precision (0.99) in identifying vulnerable snippets, minimizing false-positive alerts[cite: 2].
* **Logistic Regression** served as a solid linear baseline with 91% overall accuracy[cite: 6].
---
##  Technologies Used
* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebook[cite: 9]
* **Machine Learning & Data Processing:** Scikit-Learn, XGBoost, Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
---
##  Repository Structure
* `AI_Code_Security_Evaluator_Pipeline.ipynb` — Complete data preprocessing, model training, evaluation reports, and confusion matrix visualizations.
* `README.md` — Project documentation and experimental summary.
