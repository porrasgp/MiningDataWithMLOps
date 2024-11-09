# 📊 Data Analysis Framework

Este repositorio contiene un framework en Python para realizar un análisis completo de datos, integrando técnicas avanzadas de minería de datos y aprendizaje automático. El proyecto está estructurado para cubrir diversas técnicas, incluyendo agrupamiento, clasificación, regresión, reglas de asociación, deep learning y series de tiempo. La interfaz gráfica está desarrollada en Streamlit para facilitar la interacción y visualización de resultados.

## ✨ Características

El framework incluye los siguientes módulos:

- **🔍 Análisis No Supervisado**: Implementa técnicas como PCA, K-means, agrupamiento jerárquico, t-SNE y UMAP.
- **📈 Clasificación (Supervisado)**: Incluye algoritmos como K-Nearest Neighbors, Árboles de Decisión, Random Forest, XGBoost y AdaBoost.
- **📉 Regresión**: Modelos de regresión lineal, Lasso, Ridge y Random Forest Regression.
- **🔗 Reglas de Asociación**: Algoritmo Apriori para descubrir relaciones en grandes conjuntos de datos.
- **🤖 Deep Learning**: Configuración y entrenamiento de redes neuronales con múltiples capas.
- **📆 Series de Tiempo**: Modelos Holt-Winters y ARIMA para análisis temporal.

## 📂 Estructura del Proyecto

data_analysis_framework/
│
├── framework/
│   ├── unsupervised.py       # 🔍 Análisis no supervisado (PCA, K-means, etc.)
│   ├── supervised.py         # 📈 Clasificación (KNN, Árboles de decisión, etc.)
│   ├── regression.py         # 📉 Regresión (lineal, Lasso, Ridge, etc.)
│   ├── association.py        # 🔗 Reglas de asociación (Apriori)
│   ├── deep_learning.py      # 🤖 Deep Learning (redes neuronales)
│   ├── time_series.py        # 📆 Series de tiempo (Holt-Winters, ARIMA)
│   └── data_loader.py        # 📂 Carga de datos de SQL/NoSQL o sitios web
│
├── frontend/
│   └── app.py                # 🌐 Interfaz gráfica en Streamlit
│
├── tests/                    # ✅ Pruebas unitarias
│   ├── test_unsupervised.py
│   ├── test_supervised.py
│   └── ...
│
└── README.md                 # 📝 Descripción del proyecto



## ⚙️ Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tuusuario/data_analysis_framework.git
   cd data_analysis_framework


🚀 UsoEjecución de la Interfaz Gráfica
Inicia la aplicación gráfica en Streamlit para interactuar con el framework:


streamlit run frontend/app.py
Ejemplo de Uso
Puedes importar y usar los módulos en tus scripts de Python para análisis específicos. Ejemplo de un análisis de PCA:


from framework.unsupervised import UnsupervisedAnalysis
import pandas as pd

# Cargar datos de ejemplo
data = pd.read_csv("data.csv")
analysis = UnsupervisedAnalysis(data)
pca_result = analysis.pca(n_components=2)
✅ Pruebas

Este proyecto incluye pruebas unitarias para cada módulo. Para ejecutarlas:
Copiar código
python -m unittest discover tests

🤝 Contribución
¡Las contribuciones son bienvenidas! Si tienes ideas o encuentras algún problema, abre un issue o envía un pull request.

📜 Licencia
Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.




