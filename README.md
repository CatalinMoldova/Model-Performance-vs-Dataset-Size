# Model-Performance-vs-Dataset-Size



## 🧠 Overview

This notebook explores how training data size influences model performance. Using a dataset retrieved from **OpenML (ID: 1492)**, it walks through data analysis, model training, and performance evaluation with two different classifiers.

The notebook is divided into **three main parts**:

1. **Dataset exploration and visualization**
2. **Model training and evaluation**
3. **Performance analysis across subsets of data**

---

## 📦 Dependencies

Make sure you have the following Python packages installed before running the notebook:

```bash
pip install openml pandas numpy scikit-learn matplotlib seaborn
```

---

## 🧩 Dataset

* **Source:** OpenML Dataset ID 1492
* **Description:** The dataset is balanced with an equal number of instances (16 per class).
* **Features:** The data and target variables are automatically extracted from the OpenML dataset.

---

## ⚙️ Workflow

### **Part 1: Dataset Exploration**

* Loads the dataset from OpenML.
* Inspects class balance and structure using `Counter` and pandas summaries.
* Visualizes the class distribution using a Seaborn bar plot.

### **Part 2: Model Training**

* Splits data into **training** and **testing** sets (80/20).
* Trains two models on progressively larger subsets of the training data:

  * `DecisionTreeClassifier`
  * `GradientBoostingClassifier`
* Tracks and records model accuracy and training time.

### **Part 3: Results Analysis**

* Results are collected into a pandas `DataFrame` for easy inspection.
* Enables comparison between model performance and training time as dataset size increases.

---

## 📈 Output

Expected outputs include:

* Class distribution bar plot
* Table (`DataFrame`) with columns for subset size, accuracy, and training time
* Possible insights on model scalability

---

## 🧪 Example Run

To execute all cells:

```bash
jupyter notebook Catalin_Botezat_cb5330_problem2_HW1.ipynb
```

Or from within Python:

```python
!jupyter nbconvert --to notebook --execute Catalin_Botezat_cb5330_problem2_HW1.ipynb
```

---

## 🗂️ File Structure

```
Catalin_Botezat_cb5330_problem2_HW1.ipynb
README.md
```

---

## 🧾 License

This notebook is provided for educational purposes as part of a machine learning coursework assignment.

---
