# Mall Customer Segmentation with K-Means

## 📌 Project Overview
This project applies **K-Means clustering** to the **Mall Customers dataset** to group customers into distinct segments based on their **Annual Income** and **Spending Score**.  
The goal is to identify patterns in customer behavior for targeted marketing strategies.

---

## 📊 Dataset
- **Source**: Mall Customers dataset ([Kaggle Link](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python))
- **Features**:
  - `CustomerID`: Unique customer identifier
  - `Gender`: Male/Female
  - `Age`: Age of the customer
  - `Annual Income (k$)`: Annual income in thousands of dollars
  - `Spending Score (1-100)`: Score assigned by the mall based on customer spending patterns

---

## 🔍 Steps Performed

### 1. Exploratory Data Analysis (EDA)
- Checked for missing values and dataset info
- Descriptive statistics
- Visualizations:
  - Gender distribution
  - Age distribution
  - Annual Income distribution
  - Spending Score distribution
  - Pairplot for feature relationships

### 2. Data Preprocessing
- Selected `Annual Income` and `Spending Score` for clustering
- Standardized features using **StandardScaler**

### 3. Model Building
- Used the **Elbow Method** to determine optimal `k`
- Applied **K-Means** clustering with `k=5`
- Assigned cluster labels to customers

### 4. Evaluation
- **Silhouette Score** calculated to assess clustering quality
- Visualized customer segments with color-coded clusters

---

## 📈 Results
- **Optimal k** found to be `5` using the Elbow Method
- **Silhouette Score**: ~0.555
- Clusters indicate distinct groups of customers based on income and spending behavior

---

## 📂 Repository Structure
├── Mall_Customers.csv # Dataset file
├── Task8_KMeans_EDA.py # Python script with full code
├── Mall_Customers_Clustered.csv # Output with cluster labels
└── README.md # Project documentation



---

## 🚀 How to Run
1. Clone the repository:
```bash
- git clone https://github.com/yourusername/mall-customer-segmentation-kmeans.git

2 .Install dependencies:

- pip install pandas numpy matplotlib seaborn scikit-learn


3. Run the script:

- python Task8_KMeans_EDA.py
