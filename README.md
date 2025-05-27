# 🛳️ Titanic Dataset Analysis

This project analyzes the Titanic dataset using Python in a Jupyter Notebook. It covers data cleaning, handling missing values, correcting column names, and visualizing survival distribution.

---

## 📁 Dataset

- The dataset file: `titanic.csv`
- Contains passenger data such as age, sex, class, and survival status.
- Note: The dataset had a typo in the survival column name (`2urvived`), which is corrected in the code.

---

## 🧰 Technologies Used

- Python
- Pandas (data manipulation)
- Matplotlib & Seaborn (data visualization)
- Jupyter Notebook (interactive analysis)

---

## 📊 Analysis Steps

1. Load the Titanic dataset.
2. Rename the incorrect column (`2urvived` → `Survived`).
3. Check for missing values before cleaning.
4. Handle missing values:
   - Fill numeric columns with their mean.
   - Fill categorical columns with their mode.
5. Check missing values after cleaning.
6. Visualize survival distribution using a pie chart.

---

## 📷 Visualization Preview

When running the notebook, the survival distribution pie chart displays **inline** as output, showing the proportion of passengers who survived vs. those who did not.

Example code snippet for the pie chart:

```python
plt.pie(survival_counts, labels=labels, autopct='%1.1f%%', colors=colors, startangle=90, explode=[0, 0.1])
plt.title('Survival Distribution in Titanic Dataset')
plt.show()
