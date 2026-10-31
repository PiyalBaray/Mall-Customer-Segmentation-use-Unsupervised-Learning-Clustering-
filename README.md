#  Mall Customer Segmentation Using Machine Learning

##  Project Overview

Mall Customer Segmentation is an Unsupervised Machine Learning project that groups customers based on their shopping behavior, annual income, age, and spending score.

The main objective of this project is to identify different customer segments using clustering algorithms so that businesses can better understand customer behavior and develop effective marketing strategies.

An interactive web application is also developed using **Gradio**, where users can enter customer details and predict their customer segment.

##  Project Objectives

- Analyze customer shopping behavior.
- Identify different customer groups using clustering techniques.
- Understand the relationship between annual income and spending score.
- Compare different clustering algorithms.
- Select an appropriate clustering model.
- Build an interactive customer segmentation web application.

##  Dataset Information

**Dataset:** Mall Customers Dataset

**Total Records:** 200

**Total Features:** 5

| Feature | Description |
|---|---|
| CustomerID | Unique customer identification number |
| Gender | Customer gender |
| Age | Customer age |
| Annual Income (k$) | Customer annual income |
| Spending Score (1-100) | Customer spending score |

##  Data Preprocessing

The following preprocessing steps were performed:

- Data Loading
- Data Inspection
- Missing Value Checking
- Duplicate Value Checking
- Data Type Checking
- Exploratory Data Analysis (EDA)
- Feature Selection
- Feature Scaling using StandardScaler

### Selected Features

1. Age
2. Annual Income (k$)
3. Spending Score (1-100)

`CustomerID` was excluded because it is only an identifier. `Gender` was not included in the selected model features.

##  Exploratory Data Analysis (EDA)

The following visualizations were performed:

- Gender Distribution
- Age Distribution
- Annual Income Distribution
- Spending Score Distribution
- Boxplots for Outlier Analysis
- Annual Income vs Spending Score
- Correlation Heatmap

##  Machine Learning Algorithms

The project explores the following clustering algorithms:

1. K-Means Clustering
2. Hierarchical Clustering
3. DBSCAN
4. Mean Shift
5. Gaussian Mixture Model (GMM)

### Final Model

**K-Means Clustering**

K-Means was selected for the final customer segmentation workflow based on the model comparison and evaluation performed during the project.

The optimal number of clusters was investigated using:

- Elbow Method
- Silhouette Score

##  Model Evaluation Metrics

The clustering models were evaluated using:

| Metric | Purpose |
|---|---|
| Silhouette Score | Measures cluster separation and cohesion |
| Davies-Bouldin Score | Measures similarity between clusters |
| Calinski-Harabasz Score | Measures cluster separation |

**Metric Interpretation:**

- Higher Silhouette Score is generally better.
- Lower Davies-Bouldin Score is generally better.
- Higher Calinski-Harabasz Score is generally better.

## Customer Segmentation

Customers are grouped into four broad business categories based on average income and spending score:

| Customer Segment | Description |
|---|---|
| High Income - High Spending | Customers with high income and high spending scores |
| High Income - Low Spending | Customers with high income but low spending scores |
| Low Income - High Spending | Customers with low income but high spending scores |
| Low Income - Low Spending | Customers with low income and low spending scores |

Note: Depending on the selected K value, multiple clusters may belong to the same broad business category.

##  Web Application

An interactive web application was developed using **Gradio**.

### Application Features

- Customer Age Input
- Annual Income Input
- Spending Score Input
- Predict Customer Segment
- Display Predicted Cluster
- Display Customer Segment
- About Project Section
- Contact Section

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Scikit-learn | Machine Learning |
| Joblib | Model Saving and Loading |
| Gradio | Web Application |
| Google Colab | Development Environment |
| GitHub | Project Hosting |

##  Project Structure

```text
Mall-Customer-Segmentation/
│
├── Mall_Customers.csv
│
├── Mall_Customer_Segmentation.ipynb
│
├── final_kmeans_model.pkl
├── customer_scaler.pkl
├── segment_names.pkl
│
├── app.py
│
├── requirements.txt
│
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Mall-Customer-Segmentation.git
```

### 2. Navigate to the Project Folder

```bash
cd Mall-Customer-Segmentation
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 4. Run the Gradio Application

```bash
python app.py
```

##  Requirements

Create a `requirements.txt` file with the following libraries:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
gradio
joblib
```

## 💾 Saved Model Files

The following trained files are used by the Gradio application:

- `final_kmeans_model.pkl` — Trained K-Means model.
- `customer_scaler.pkl` — Fitted StandardScaler.
- `segment_names.pkl` — Customer segment mapping.

## 🔮 Future Improvements

- Improve customer segmentation using additional features.
- Compare clustering algorithms with further parameter tuning.
- Build a more advanced interactive dashboard.
- Deploy the application online.
- Add customer behavior insights and business recommendations.

## 👨‍💻 Author

**Piyal Baray**

**Email:** piyalbaray314@gmil.com

##  Support

If you find this project useful, please consider giving this repository a  on GitHub.

---

**Made with  using Python and Machine Learning.**
