# UN Global Terrorism Analysis ML Unsupervised Learning and PowerBI Dashboard

# 📌 Project Overview
This project presents a comprehensive analysis of global terrorism incidents using unsupervised machine learning and interactive Power BI dashboards. This project focuses on identifying terrorism-prone geographical regions (hotspots) using unsupervised machine learning techniques. Instead of manually defining how many clusters (regions) exist, the system automatically detects natural groupings in the data.
The approach combines:

* Density-based clustering (DBSCAN) → to detect irregular hotspot regions
* K-Means (for comparison & validation)
* PCA → to reduce dimensionality and improve clustering performance

**PowerBI Dashboard Zip link pasted below.**

# Machine Learning Workflow and PowerBI Overview

<img width="864" height="1821" alt="image" src="https://github.com/user-attachments/assets/a97978d1-7619-4a0b-bfe6-73cde9840de9" />


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

# 🔍 Exploratory Data Analysis (EDA)
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

<img width="310" height="162" alt="image" src="https://github.com/user-attachments/assets/4f08bc64-05de-42bd-bbb3-5dc325109293" />


# **Power BI Dashboard zip Link**
https://drive.google.com/file/d/1O3TNYpaj13lUirKwaj85hzUQMdyWgvFr/view?usp=sharing

The Power BI dashboard is divided into two main pages:

# 📍 Page 1 — EDA Dashboard

<img width="1306" height="746" alt="Screenshot 2026-04-26 110737" src="https://github.com/user-attachments/assets/7a1f4ab9-d49d-4712-bc34-f842c803f58d" />

# **Cards**
* Total Incidents
* Total Casualties
* Affected Countries

# **Slicers**
* Countries
* Type of attacks
* Year

# **Visualizations**
* Attacks per Year (Line Chart)
* Global Attack Map
* Top Countries (Bar Chart)
* Attack Type Distribution (Donut Chart)
* Region-wise Analysis

# 📍 Page 2 — Machine Learning Dashboard

<img width="1308" height="742" alt="Screenshot 2026-04-26 110856" src="https://github.com/user-attachments/assets/4779a93c-d52e-4589-994b-8d7efa7af3c1" />

# **Slicers**
* Countries
* Region

# **Visualizations**
* Global Attack Hotspot Map
* Top Regions (Column Chart)
* Type of Attacks (Bar Chart)
* Total Attacks (Cluster based)

# 📈 Machine Learning Insights
* Terrorism incidents are not random
* They are concentrated in specific hotspots
* Some areas consistently show high activity
* There are rare isolated attacks (outliers)
* Patterns are irregular and complex

# 🛠️ Technologies Used
**Programming**
* Python
* Pandas
* NumPy

**Machine Learning**
* KMeans
* PCA
* DBSCAN

**Visualization**
* Matplotlib
* Seaborn
* Power BI

# 🚀 Key Achievement
* DBSCAN identifies natural terrorism hotspots on maps
* Activities are clustered, not random
* Noise points represent isolated incidents
* K-Means gives forced clusters; DBSCAN is more accurate
* Power BI dashboard enables interactive maps and filters
* Hotspots change over time (dynamic patterns)
* Some regions show high frequency, others high severity
* Attack patterns vary by region
* Overall, dashboard converts ML output into clear, actionable insights

# 📌 Conclusion
* Hotspots detected using unsupervised learning (no predefined clusters)
* DBSCAN is best: handles noise + finds natural clusters
* K-Means is less effective due to fixed clusters
* Power BI makes insights visual and interactive
* Terrorism is concentrated and dynamic
* Requires continuous monitoring
* Helps in resource allocation, risk analysis, and planning
* Final: ML + Power BI creates a strong decision-support system
