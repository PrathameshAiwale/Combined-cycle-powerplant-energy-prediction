# Combined Cycle Power Plant Energy Prediction
Machine Learning project to predict electrical energy output of a Combined Cycle Power Plant using environmental sensor data.

## Project Overview
This project predicts the electrical energy output of a Combined Cycle Power Plant using machine learning models trained on hourly environmental sensor data.  
The dataset includes temperature, ambient pressure, relative humidity, and exhaust vacuum readings to estimate net hourly power output (in MW).

The goal is to help optimize plant operations by forecasting energy generation based on ambient conditions.

## Dataset
The dataset has 9568 hourly samples with these features:

| Feature                       | Description                     | Range                 |
|-------------------------------|---------------------------------|-----------------------|
| Temperature (T)               | Ambient temperature (°C)        | 1.81 to 37.11         |
| Ambient Pressure (AP)         | Atmospheric pressure (milibar)  | 992.89 to 1033.30     |
| Relative Humidity (RH)        | Relative humidity (%)           | 25.56 to 100.16       |
| Exhaust Vacuum (V)            | Exhaust vacuum pressure (cm Hg) | 25.36 to 81.56        |
| Electrical Energy Output (PE) | Net hourly power output (MW)    | 420.26 to 495.76      |

## Methodology

- Loaded and explored the data in Google Colab.
- Split data into features (inputs) and target (output).
- Divided data into training and test sets (80-20 split).
- Standardized features for better model performance.
- Built and compared two regression models:
  - Linear Regression
  - Random Forest Regressor
- Evaluated models using RMSE (Root Mean Squared Error) and MAE (Mean Absolute Error).
- Selected Random Forest as the final model due to better accuracy.

## How to Run

1. Open the project notebook directly in Google Colab by clicking https://colab.research.google.com/drive/1AziB_eB6BieaIIOILyMdy6kWPVKnYQDe?usp=sharing

2. Upload the dataset file (`powerplant.csv`) to the Colab environment:
   - Click the folder icon on the left panel in Colab.
   - Click the upload icon and select your CSV file.

3. Run all notebook cells sequentially to reproduce data preprocessing, model training, evaluation, and visualization.

## Results Summary

| Model             | RMSE (MW) | MAE (MW) |
|-------------------|-----------|----------|
| Linear Regression | ~4.5      | -        |
| Random Forest     | ~3.25     | 2.33     |

The Random Forest model shows better performance in predicting electrical energy output.

## Project Files

- `powerplant_energy_prediction.ipynb` — The full Colab notebook with code and explanations.
- `powerplant.csv` — Dataset file
  
## About the Author

**Prathamesh** — Aspiring Data Scientist and Machine Learning Engineer  
[LinkedIn](http://www.linkedin.com/in/pr4th4m35h) | [Portfolio](www.prathameshaiwale.com)

---

## License

This project is licensed under the MIT License.

