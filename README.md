Predicción de Carreras (Runs) en Béisbol - MLB 2008

Modelo de regresión con Random Forest para predecir el número de carreras anotadas usando únicamente el número de bateos.

Resultados finales

R² en test: 0.804
RMSE: 37.12
MAE: 31.45

import joblib
modelo = joblib.load('best_rf_model.pkl')
print(modelo.predict([[5600]]))  # ejemplo: 5600 bateos → ~750 runs
