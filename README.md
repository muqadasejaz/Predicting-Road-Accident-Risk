# 🚗 Predicting Road Accident Risk  

 **Data-driven prediction of accident likelihood based on road, environmental, and situational factors.**  
 Built using **LightGBM**, **Python**, and **Kaggle Playground Series S5E10** dataset.  

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🧠 Project Overview

This project focuses on predicting the **number of reported road accidents** using a variety of influencing factors such as:
- Road type, speed limit, and curvature  
- Lighting and weather conditions  
- Time of day and holiday information  
- School season and public road status  

The model helps to estimate **accident risk** under different real-world conditions, contributing to **safer road planning and policy-making** through data-driven insights.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## ✨ Features

- 📊 **Exploratory Data Analysis (EDA)**: Visual exploration of distributions, correlations, and outliers.  
- 🧩 **Feature Engineering**: Created derived features like `lanes_over_speed`, `curvature_over_lanes`, and `is_high_speed`.  
- ⚙️ **Model Training**:  Used **LightGBM** (Gradient Boosting Decision Tree) with K-Fold Cross Validation.  
- 🔁 **Cross Validation (5-Fold)**:  Ensures robust generalization and performance evaluation.  
- 📉 **Outlier Detection**: Used boxplots for numeric features to identify and handle outliers.  
- 📈 **Feature Importance Plot**: Highlights the most influential factors impacting accident likelihood.  
- 🧾 **Kaggle Submission Pipeline**: Generates final `submission.csv` automatically.  

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🛠️ Tools and Technologies

| Category | Tools / Libraries |
|-----------|------------------|
| **Programming Language** | Python 3.10+ |
| **Machine Learning** | LightGBM, Scikit-learn |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Seaborn, Matplotlib |
| **Environment** | Kaggle Notebook / Jupyter |
| **Evaluation Metrics** | RMSE, MAE |

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📂 Dataset

**Source:** [Kaggle Playground Series — Season 5 Episode 10](https://www.kaggle.com/competitions/playground-series-s5e10/data)

| Column | Description |
|---------|-------------|
| `id` | Unique identifier |
| `road_type` | Type of road (urban, rural, highway, etc.) |
| `num_lanes` | Number of lanes |
| `curvature` | Road curvature measurement |
| `speed_limit` | Speed limit of the road |
| `lighting` | Lighting condition (daylight, night, etc.) |
| `weather` | Weather condition |
| `road_signs_present` | Presence of road signs |
| `public_road` | Indicates if road is public |
| `time_of_day` | Time period (morning, night, etc.) |
| `holiday` | Whether it was a public holiday |
| `school_season` | Whether schools were in session |
| `num_reported_accidents` | Target variable (number of accidents) |

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📈 Results

| Metric | Mean | Std |
|---------|------|-----|
| **CV RMSE** | 0.8806 | 0.0006 |
| **CV MAE** | 0.6837 | 0.0010 |
| **Model Used** | LightGBM Regressor |
| **Validation Strategy** | 5-Fold Cross Validation |

**Interpretation:**  
A lower RMSE and MAE indicate that the model accurately captures accident trends based on environmental and road conditions.  
Further improvements can be achieved by advanced feature engineering or ensemble models (CatBoost/XGBoost blending).

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🖼️ Visual Insights

| Plot | Description |
|------|-------------|
| **Boxplots** | Detects outliers in numeric features (speed limit, curvature, etc.) |
| **Histograms** | Displays feature and target distributions |
| **Feature Importance** | Shows top predictors influencing accident risk |
| **True vs Predicted** | Scatter plot comparing predicted vs actual accident counts |

- Histogram:

<img width="1390" height="990" alt="image" src="https://github.com/user-attachments/assets/793472a5-b3d5-46f1-9029-15861ebeff9a" />

<img width="989" height="390" alt="image" src="https://github.com/user-attachments/assets/61703420-4bab-4242-a08c-1feb166e9b8e" />

- CountPlots:
  
<img width="1585" height="1190" alt="image" src="https://github.com/user-attachments/assets/32490914-7e37-4425-aa89-8beea5cefc58" />

- Boxplots:
  
<img width="822" height="528" alt="image" src="https://github.com/user-attachments/assets/9fa6c459-5d7b-4833-8da6-a2b575d6a1a5" />


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🔮 Future Work

- 🧠 Implement **CatBoost** or **XGBoost** for model comparison.  
- 🔍 Explore **zero-inflated regression** (for rare accident counts).  
- 🌐 Build an **interactive dashboard** to visualize accident risk zones.  
- 🚀 Deploy a **Flask web app** for real-time accident risk estimation.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📚 References

1. [Kaggle Playground Series — S5E10](https://www.kaggle.com/competitions/playground-series-s5e10/overview)  
2. [LightGBM Documentation](https://lightgbm.readthedocs.io/en/latest/)  
3. [Scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)  
4. [Seaborn Visualization Tutorial](https://seaborn.pydata.org/tutorial.html)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 👤 Author

Muqadas Ejaz

BS Computer Science (AI Specialization)

AI/ML Engineer

Data Science & Gen AI Enthusiast

📫 Connect with me on [LinkedIn](https://www.linkedin.com/in/muqadasejaz/)  

🌐 GitHub: [github.com/muqadasejaz](https://github.com/muqadasejaz)

📬 Kaggle: [Kaggle Profile](https://www.kaggle.com/muqaddasejaz) 

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📎 License

This project is open-source and available under the [MIT License](LICENSE).
