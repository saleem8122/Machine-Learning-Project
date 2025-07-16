# Machine-Learning-Project


🧠 K-Means Clustering to Group Products Based on Popularity and Price
📘 Project Title
Product Segmentation Using K-Means Clustering Based on Popularity and Price

📋 Objective
The goal of this project is to apply K-Means clustering, an unsupervised machine learning algorithm, to group products from an online sales dataset based on:

📈 Popularity (how often a product was purchased)

💰 Average Price

This helps identify similar products, uncover market segments, and support better pricing and marketing strategies.

📁 Dataset Overview
The dataset used is "Online Sales Data.csv", which includes:

Transaction ID – unique ID per purchase

Product Name – the name of each product

Unit Price – price per unit sold

Other fields like Date, Product Category, Region, Payment Method

🧹 Data Preprocessing
Dropped missing values in key columns: Product Name, Unit Price, Transaction ID

Ensured Unit Price is numeric

Grouped the dataset by Product Name to compute:

Popularity = number of transactions per product

Average Price = average unit price per product

📏 Feature Scaling
Used StandardScaler to normalize Popularity and Average Price so they can be used fairly in clustering.

🤖 Model: K-Means Clustering
Applied K-Means algorithm to cluster products based on the two features:

Popularity

Average Price

Used Silhouette Score to find the optimal number of clusters (k) ranging from 2 to 10.

📊 Cluster Evaluation
Silhouette Score was used to evaluate clustering performance:

Measures how well points fit within their own clusters and how separated the clusters are.

Score ranges from -1 to +1, with values near +1 indicating good clustering.

📈 Visualization
Plotted the clusters using Seaborn to visually inspect how products are grouped based on popularity and price.

Each product is color-coded by its cluster.

💡 Insights from Clusters
For each cluster, we identified:

Top 5 most popular products

Average price and popularity of the group

Useful for understanding:

🧲 Low-cost high-selling products

💎 High-priced niche products

📦 Medium-tier mainstream products

📤 Output
The final output is saved as Clustered_Products.csv

This includes:

Product Name

Popularity

Average Price

Assigned Cluster

✅ Technologies Used
Tool/Library	Purpose
Python	Programming language
Pandas	Data cleaning and grouping
Scikit-learn	Machine learning (KMeans, scaling, evaluation)
Seaborn / Matplotlib	Data visualization
Google Colab	Development environment

🎯 Use Cases / Applications
📦 Product categorization in e-commerce platforms

🎯 Targeted marketing based on pricing tiers

📈 Dynamic pricing strategy planning

🛍️ Inventory management based on demand clusters
