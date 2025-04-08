# 📈 Predicción del Índice S&P 500 con Modelos de Machine Learning

Este proyecto tiene como objetivo predecir el retorno diario del índice S&P 500 utilizando precios históricos de acciones, datos sectoriales y variables financieras agregadas. 

La solución se construyó con un enfoque profesional de ciencia de datos, incluyendo limpieza de datos, EDA, ingeniería de características y evaluación de múltiples modelos.

---

## 📁 Estructura del Proyecto

- `notebooks/`: análisis exploratorio, generación de features y entrenamiento de modelos.
- `data/`
- `reports/`: visualizaciones y resultados de los modelos.
- `requirements.txt`: librerías necesarias para reproducir el proyecto.

---

## ⚙️ Tecnologías usadas

- Python (Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn)
- XGBoost
- Jupyter Notebook
- Git + GitHub

---

## 🧪 Modelos entrenados

| Modelo              | MAE     | RMSE    | R²     |
|---------------------|---------|---------|--------|
| Regresión Lineal    | 0.00132 | 0.00180 | 0.9506 |
| Random Forest       | 0.00245 | 0.00322 | 0.8428 |
| XGBoost             | 0.00237 | 0.00306 | 0.8579 |
| Gradient Boosting   | 0.00247 | 0.00316 | 0.8480 |

---
# 📂 Instrucciones para Obtener los Datos

Este proyecto utiliza el dataset **"S&P 500 Stocks - Daily Updated"** disponible en Kaggle:

🔗 https://www.kaggle.com/datasets/andrewmvd/sp-500-stocks

---

## ✅ Cómo descargar los datos

1. Asegúrate de tener una cuenta en [Kaggle](https://www.kaggle.com/).
2. Instala la API de Kaggle si no la tienes:
   ```bash
   pip install kaggle
   ```
3. Coloca tu archivo `kaggle.json` (con tu API Token de Kaggle) en la carpeta `~/.kaggle/`.  
   Puedes descargarlo desde: https://www.kaggle.com/account

4. Verifica o configura el path con:
   ```bash
   kaggle config set -n path -v ~/.kaggle/
   ```

5. Descarga y descomprime los datos directamente en la carpeta `data/` del proyecto:
   ```bash
   kaggle datasets download -d andrewmvd/sp-500-stocks -p data --unzip
   ```

---

## 📄 Archivos esperados

Después de la descarga, asegúrate de tener estos archivos dentro del directorio `data/`:

- `sp500_stocks.csv`
- `sp500_index.csv`
- `sp500_companies.csv`

---
