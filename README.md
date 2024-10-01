# UHI Effect Analysis and Mitigation

## Project Overview

This project aims to analyze and mitigate the Urban Heat Island (UHI) effect in urban zones by studying various environmental factors. The UHI effect leads to increased temperatures in urban areas compared to their rural surroundings, primarily due to human activities and urban infrastructure. The goal of this project is to provide actionable insights to reduce the UHI effect and improve environmental conditions in affected areas.

Our team focused on identifying the UHI effect using a combination of cluster-based analysis and machine learning techniques. The analysis helps to categorize urban areas into clusters based on factors such as green cover, water bodies, building density, and current/future temperature trends. Based on this categorization, we provide recommendations for mitigating the UHI effect in each cluster.

## Key Features

- **Cluster-Based Analysis:** Urban areas are categorized into clusters based on environmental features such as:
  - Water body percentage
  - Green area percentage
  - Building density
  - Current and future temperatures
  
- **Weather Prediction using LSTM:** Time series forecasting using Long Short-Term Memory (LSTM) networks to predict future temperature trends for different zones.
  
- **Mitigation Recommendations:** For each cluster, we propose strategies to mitigate the UHI effect, considering factors like building density, green spaces, and water bodies.

## Methodology

1. **Data Collection:**
   - Data includes features like solar radiation, humidity, dew point, temperature max/min, cloud cover, and environmental factors like water body percentage, green area, and building density.
   - The data is clustered to identify zones with similar environmental conditions.

2. **Clustering:**
   - Areas are grouped into clusters based on the mentioned environmental factors. Each cluster exhibits specific characteristics contributing to the UHI effect.
   
3. **Modeling & Prediction:**
   - **LSTM for Temperature Prediction:** LSTM models were used to predict future temperature trends in each zone based on historical weather data.
   
4. **Recommendations:**
   - General recommendations are provided to mitigate UHI effects, focusing on increasing green spaces, optimizing water body distribution, and reducing heat-retaining infrastructure.

## Project Structure
```
UHI-Effect-Analysis-and-Mitigation/
│
├── data/                                  # Contains datasets for each zone
│   ├── Adyar.csv                          # Dataset for Adyar zone
│   ├── AnnaNagar.csv                      # Dataset for Anna Nagar zone
│   ├── Manali.csv                         # Dataset for Manali zone
│   ├── ...                                # Other zone datasets (total 14)
│
├── models/                                # Trained models
│   └── random_forest_temp_prediction_model.pkl  # Random forest model for temperature prediction
│
├── notebooks/                             # Jupyter Notebooks with analysis code                
│   ├── UHI_INDEX with temp pred_greenarea_waterbody_building_density.ipynb # Main code for processing temperature data and predictions
│   └── UHIEffect_Mitigation.ipynb         # Cluster analysis and mitigation
└── 
```



## Technologies Used

- **Python** for data analysis and machine learning
- **Scikit-learn** and **TensorFlow/Keras** for clustering and predictive modeling
- **Pandas** and **NumPy** for data manipulation
- **Matplotlib** and **Seaborn** for visualization
- **Jupyter Notebooks** for prototyping and development

    We applied machine learning techniques to predict temperature trends and used clustering to categorize areas based on environmental characteristics. 

## License

[MIT License](LICENSE)

