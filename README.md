🛍️ Mall Customer Segmentation Project
🎯 Objective:
Cluster customers into meaningful segments based on Annual Income and Spending Score to support targeted marketing strategies.

📁 Dataset Used:
Mall_Customers.csv from Kaggle
Includes:
— Customer ID
— Gender
— Age
— Annual Income (k$)
— Spending Score (1–100)

🔍 Step-by-Step Workflow:

1️⃣ Feature Selection
Focused on the two most relevant features for clustering:
— Annual Income
— Spending Score

2️⃣ Data Scaling
Applied StandardScaler to normalize the data and ensure better clustering results.

📊 K-Means Clustering

✅ Elbow Method:
Used to determine the optimal number of clusters — found 5 clusters.

✅ Model Applied:
K-Means with n_clusters=5.

✅ Results & Insights:

Cluster 0: Income ≈ 55.3k, Score ≈ 49.5 → 🎯 Average spenders

Cluster 1: Income ≈ 86.5k, Score ≈ 82.1 → 💸 High-income, high-spending customers

Cluster 2: Income ≈ 25.7k, Score ≈ 79.4 → 🧭 Low-income, high-spending customers

Cluster 3: Income ≈ 88.2k, Score ≈ 17.1 → 💰 High-income, low-spending customers

Cluster 4: Income ≈ 26.3k, Score ≈ 20.9 → 🧍 Low-income, low-spending customers

🔎 DBSCAN Clustering

✅ Parameters Used:
eps = 0.5, min_samples = 5

✅ Results & Insights:

Cluster 0: Income ≈ 52.5k, Score ≈ 43.1 → 🌐 Core customer group

Cluster 1: Income ≈ 82.5k, Score ≈ 82.8 → 🏆 Elite spenders

Noise Points: 8 customers identified as outliers (Cluster -1)

🧠 Conclusion:
K-Means produced well-separated, interpretable segments perfect for targeted campaigns.
DBSCAN added value by identifying dense groups and highlighting 8 outlier customers who may require unique strategies.
These insights help tailor promotions — for example, focus efforts on Cluster 1 (K-Means) for high Return on Investment (ROI), or try upselling to Cluster 0 with medium spenders.



#MachineLearning #DataScience #CustomerSegmentation #KMeans #DBSCAN #MarketingAnalytics #Clustering #Python #MallCustomerAnalysis #MLInternship
