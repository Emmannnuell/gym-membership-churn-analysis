# Predicción de Retención de Clientes: Machine Learning para Gimnasios

## 🎯 Objetivo del Proyecto
El objetivo principal fue desarrollar un modelo predictivo para identificar miembros de un gimnasio con riesgo de cancelar su suscripción (Churn). Anticipar este comportamiento permite a la administración implementar estrategias de lealtad proactivas.

## 🛠️ Herramientas Utilizadas
* **Python (Pandas, NumPy):** Procesamiento de datos y Feature Engineering.
* **Scikit-Learn:** Implementación de modelos de clasificación (**Random Forest** y **Regresión Logística**).
* **Matplotlib & Seaborn:** Análisis de correlación y visualización de perfiles de clientes.

## 📈 Metodología y Hallazgos
Se analizaron variables como frecuencia de asistencia, edad, duración del contrato y uso de servicios adicionales.

### Factores Determinantes del Abandono:
1. **Frecuencia Mensual:** Los clientes con menos de 2 visitas semanales en el último mes tienen una probabilidad de churn drásticamente mayor.
2. **Tipo de Contrato:** Los contratos mes a mes son los más volátiles en comparación con los anuales.
3. **Edad:** Los usuarios más jóvenes presentan una tasa de rotación ligeramente superior.

### 🏆 Rendimiento del Modelo
Tras comparar varios modelos, el algoritmo de Random Forest fue seleccionado por su equilibrio entre precisión y sensibilidad:
* **Accuracy:** [92%]
* **F1-Score (Clase Churn):** [0.85]

> **Impacto:** Con este modelo, el gimnasio puede identificar al **85% de los clientes en riesgo** antes de que cancelen, permitiendo acciones de retención dirigidas.

## 📂 Estructura del Repositorio
* `gym_churn_analysis.ipynb`: Notebook con el flujo completo de ML (EDA, Preprocesamiento, Modelado).
* `datasets/`: Datos históricos procesados.
