# Titanic Dataset - Exploratory Data Analysis (EDA)

This project performs **Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover patterns and insights related to passenger survival using various data visualization tools like **Matplotlib**, **Seaborn**, and **Plotly**.

---

## 📁 Dataset

* **Source:** `Titanic-Dataset.csv`
* **Features used:**

  * `Survived`, `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`
  * Engineered: `FamilySize`, `IsAlone`, `AgeGroup`

---

## 🧹 Data Preprocessing

* Missing values handled:

  * `Age` filled with **median**
  * `Embarked` filled with **mode**
* Dropped columns: `Cabin`, `Name`, `Ticket`, `PassengerId`
* Categorical conversion: `Survived`, `Sex`, `Embarked`, `Pclass`, `AgeGroup`, `IsAlone`
* Engineered Features:

  * `FamilySize = SibSp + Parch + 1`
  * `IsAlone = True` if `FamilySize == 1`
  * `AgeGroup` categorized into: Child, Teen, YoungAdult, Adult, Senior

---

## 📊 Visualizations

### 1. Distribution Plots

* Histograms for all numeric features with KDE (e.g., Age, Fare, SibSp, Parch, FamilySize)

### 2. Boxplots

* Boxplots comparing `Age`, `Fare`, `FamilySize` across `Survived` classes

### 3. Correlation Heatmap

* Shows correlation between numeric variables using Seaborn heatmap

### 4. Pairplot

* Plots pairwise relationships between `Age`, `Fare`, and `FamilySize` colored by `Survived`

### 5. Plotly Interactive

* Interactive histogram: `Pclass` vs `Sex` faceted by `Survived`
* Interactive scatter plot: `Age` vs `Fare` colored by `Survived`

---

## 🔍 Key Insights

* **Females** and **1st class** passengers had the highest survival rates.
* **Children** and **young adults** had better chances of survival.
* **FamilySize** between 2–4 increased survival chances; solo or large groups fared worse.
* **Fare** is strongly correlated with survival; wealthy passengers survived more.
* **Plotly** visuals support intuitive exploration of these patterns interactively.

---

## 📦 Libraries Used

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `plotly`
* `math`

---

## 🏁 How to Run

1. Ensure you have the Titanic dataset CSV file in your working directory.
2. Run the Python script in Jupyter Notebook or any Python IDE.
3. The script automatically opens interactive Plotly charts in your browser.

---

## ✍️ Author

Jenish Allen Immanuel J
EDA Project - Titanic Dataset
