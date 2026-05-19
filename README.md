# 👥 Employee Retention Analysis Using Unsupervised Learning

Segmenting employees with K-Means clustering and PCA to uncover retention risks and help HR teams take targeted action.

---

## 📌 Project Overview

Employee attrition is costly — this project uses unsupervised learning to identify distinct employee segments and understand which groups are most at risk of leaving. Rather than predicting who leaves, the goal is to **understand why**, and provide actionable recommendations per segment.

---

## 🎯 Goal & Scope

- **Goal:** Identify the different types of employees at the company and understand how attrition varies across segments
- **Approach:** Cluster employees using K-Means, visualize segments with PCA, and analyze attrition rates per cluster to generate retention recommendations


---

## 🔧 Techniques Used

| Technique | Purpose |
|-----------|---------|
| **K-Means Clustering** | Segment employees into distinct groups |
| **Elbow Method** | Identify the optimal number of clusters via inertia |
| **Silhouette Score** | Validate cluster quality |
| **PCA (2D & 3D)** | Reduce dimensionality for visualization |
| **StandardScaler** | Normalize features before clustering |
| **Heatmaps** | Interpret cluster centers |

---

## 📊 Workflow

```
1. Data Prep & EDA
       ↓
2. K-Means Clustering (with all features)
       ↓
3. PCA Visualization (Round 1)
       ↓
4. K-Means Clustering (without department dummies)
       ↓
5. PCA Visualization (Round 2 — 2D & 3D)
       ↓
6. EDA on Clusters (attrition & department breakdown)
       ↓
7. Recommendations
```

---

## 🔍 Key Findings

### Identified Employee Segments (6 Clusters)

| Cluster | Segment | Attrition Risk |
|---------|---------|----------------|
| 0 | Men who like their job | 🟢 Low |
| 1 | High-performing employees | 🟡 Medium |
| 2 | Long commuters | 🔴 High |
| 3 | Female employees | 🟢 Low |
| 4 | Senior employees | 🟢 Lowest |
| 5 | Men who dislike their job | 🔴 High |

### PCA Components (without departments)
- **PC1:** Seniority axis — higher age, job level, and income → more senior employees
- **PC2:** Satisfaction/demographics axis — left = happy in job, right = women / longer commute / high performing

---

## 💡 Recommendations

**High-attrition segments to prioritize:**

- **Long commuters** → Offer remote/hybrid work options; build an inclusive remote culture
- **Men who dislike their jobs** → Prompt managers to have 1:1 check-ins and address dissatisfaction
- **High performers** → Create clear paths to senior roles to prevent talent loss

**Low-attrition segments to study:**
- **Senior employees** → Long tenure naturally reduces attrition; use them as mentors
- **Female employees** → Investigate what's working and replicate it across other segments

---

## 🛠️ Tech Stack

- Python 3
- pandas, numpy
- scikit-learn (KMeans, PCA, StandardScaler, silhouette_score)
- matplotlib, seaborn
- mpl_toolkits (3D plotting)

---


## 📬 Contact

Feel free to connect or reach out if you have questions or feedback!
