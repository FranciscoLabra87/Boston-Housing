Predicción de Precios de Viviendas en Boston
Descripción del Proyecto
Este proyecto analiza el Boston Housing Dataset, un conjunto de datos clásico en Machine Learning y análisis inmobiliario. El objetivo es explorar los factores que influyen en el precio de las viviendas y entrenar modelos de regresión para predecir valores inmobiliarios con base en características clave.

Datos Utilizados
El dataset contiene información sobre propiedades en Boston, con variables como:

CRIM: Tasa de criminalidad per cápita.
ZN: Proporción de suelo residencial con grandes parcelas.
INDUS: Proporción de acres comerciales no minoristas.
RM: Número promedio de habitaciones por vivienda.
LSTAT: % de población con bajo nivel socioeconómico.
MEDV: Valor mediano de la vivienda (variable objetivo).
Metodología y Técnicas Utilizadas
Análisis Exploratorio de Datos (EDA)

Estadísticas descriptivas y detección de valores nulos.
Mapas de calor para visualizar correlaciones.
Gráficos de distribución para identificar patrones.
Selección de Variables

Identificación de las variables más correlacionadas con el precio (MEDV), como RM, LSTAT y PTRATIO.
Modelos de Machine Learning

Árboles de Decisión (DecisionTreeRegressor): Modelo basado en la división recursiva de datos.
Random Forest (RandomForestRegressor): Ensamble de múltiples árboles de decisión para mejorar la precisión.
Bagging Regressor (BaggingRegressor): Técnica de agregación para reducir la varianza del modelo.
Resultados y Conclusiones
Se identificaron los principales factores que influyen en el precio de las viviendas.
Se probaron diferentes modelos de ML, destacando Random Forest como el más preciso.
El modelo permite predecir precios con base en variables económicas y estructurales.
Requisitos
Para ejecutar este notebook, se requieren las siguientes librerías:

python
Copiar
Editar
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.tree import DecisionTreeRegressor
from sklearn.ensemble import RandomForestRegressor, BaggingRegressor
