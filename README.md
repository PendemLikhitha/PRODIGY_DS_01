# ProdigyInfoTech_TASK1
# TASK 1:Data Visualization: Age and Gender Distribution


This project demonstrates how to visualize the distribution of a categorical variable (gender) and a continuous variable (age) using the Adult Census dataset. The visualizations are created using pandas, matplotlib, and seaborn.

## Dataset

The dataset used in this project is the Adult Census dataset, which can be found on [Kaggle](https://www.kaggle.com/uciml/adult-census-income).

## Visualizations

1. *Age Distribution*: A histogram that shows the distribution of ages in the dataset.
2. *Gender Distribution*: A bar chart that shows the distribution of genders in the dataset.

## How to Run

1. Clone the repository.
2. Ensure you have the necessary libraries installed (pandas, matplotlib, seaborn).
3. Place the dataset (adult.csv) in the same directory as the script.
4. Run the script to generate the visualizations.

## Code

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load the dataset
df = pd.read_csv('adult.csv')

# Inspect the first few rows of the dataset
print(df.head())
```

![Screenshot 2024-07-06 215037](https://github.com/PendemLikhitha/PRODIGY_DS_01/assets/159911587/8e333156-5954-43e2-bd31-e6165d8edcfe)


```python
# Histogram for age distribution
plt.figure(figsize=(10, 6))
sns.histplot(df['age'], bins=20, kde=True, color='blue')
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.show()
```

# Bar chart for gender distribution
![Screenshot 2024-07-06 215200](https://github.com/PendemLikhitha/PRODIGY_DS_01/assets/159911587/7f3d27d0-3d31-4e7c-99c6-fc6f2853d5b2)



```python
# Bar chart for gender distribution
plt.figure(figsize=(10, 6))
sns.countplot(x='gender', data=df, palette='pastel')
plt.title('Gender Distribution')
plt.xlabel('Gender')
plt.ylabel('Count')
plt.show()
```
# Histogram for age distribution
![Screenshot 2024-07-06 215211](https://github.com/PendemLikhitha/PRODIGY_DS_01/assets/159911587/c05c142c-1ec4-4f66-bdd7-919a1fb80620)

