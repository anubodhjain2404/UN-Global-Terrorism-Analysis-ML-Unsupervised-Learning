# UN-Global-Terrorism-Analysis-ML-Unsupervised-Learning

# 📌 Project Overview
This project presents a comprehensive analysis of global terrorism incidents using unsupervised machine learning and interactive Power BI dashboards. This project focuses on identifying terrorism-prone geographical regions (hotspots) using unsupervised machine learning techniques. Instead of manually defining how many clusters (regions) exist, the system automatically detects natural groupings in the data.
The approach combines:

* Density-based clustering (DBSCAN) → to detect irregular hotspot regions
* K-Means (for comparison & validation)
* PCA → to reduce dimensionality and improve clustering performance

# Machine Learning Workflow

<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/81d6cf3f-eea8-472e-9b49-1a8a19645485" />

# 🎯 Business Objective
The main goal is to support decision-making for security and policy planning.

Key Objectives:
* Identify terrorism hotspots automatically without human bias
* Help governments allocate security forces and resources efficiently
* Detect emerging risk zones before they become major hotspots
* Support intelligence agencies in pattern recognition and threat analysis
* Enable data-driven insights for counter-terrorism strategies

# 📊 Dataset Requirements
* Latitude & Longitude → for spatial clustering
* Year → for temporal trend analysis
* Country → for mapping and interpretation
* Attack Type 
* Target Type 
* Number of Casualties 
* Weapon Type
* Terrorist group name

🔍 Exploratory Data Analysis (EDA)
**Key Insights**
* Terrorist attacks peaked around 2014
* Iraq and Afghanistan were the most affected countries
* Bombing/Explosion was the most common attack type
* Most incidents resulted in low casualties
* High severity incidents are rare but impactful

# 🤖 Machine Learning Approach
Unsupervised learning algorithms were applied to identify hidden severity patterns.

# 1️⃣ K-Means Clustering
* Data grouped into clusters based on similarity
* Some clusters show high activity regions
* Requires predefined K
* Cannot detect irregular shapes

# 2️⃣ PCA
* Data reduced to 2 components
* Helps visualize patterns clearly
* Shows separation between clusters
* Not used for clustering directly

# 3️⃣ DBSCAN Clustering
* The visualization shows that terrorism incidents are concentrated in specific dense regions (hotspots)
* DBSCAN successfully separates these hotspots from isolated events (noise)
* The clusters are irregular in shape, reflecting real-world geographical patterns
* It also highlights variation in intensity across regions, with some areas having significantly higher activity
* Identifies high-density regions (hotspots)
* Detects noise (-1) → isolated attacks
* Works without predefined clusters
* Captures real-world irregular patterns

# 🏆 Best Model Selection
**DBSCAN** is the most suitable algorithm.

**Reason:**
* No need for cluster count
* Detects dense regions
* Handles noise
* Works best for geographical data


# 📊 Power BI Dashboard

