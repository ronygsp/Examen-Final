# Churn Prediction Project – Interconnect

Este proyecto aborda el problema de predicción de cancelación de clientes (`churn`) en una empresa de telecomunicaciones, con el objetivo de anticipar bajas y permitir campañas de retención más efectivas.

## 📂 Datos Utilizados

Se trabajó con cuatro fuentes de datos:

- `contract.csv`: información contractual (7043 registros)
- `personal.csv`: datos demográficos (7043 registros)
- `internet.csv`: servicios de internet (5517 registros)
- `phone.csv`: servicios telefónicos (6361 registros)

Estas fuentes se integraron en un único dataset unificado con 7043 clientes únicos.

## 🧠 Fase de Modelado

Se derivaron nuevas variables (como `tenure`, `HasAddOns`, `ValuePerService`) y se prepararon los datos para modelos supervisados. La variable objetivo `Churn` fue generada a partir de la fecha de finalización del contrato (`EndDate`).

Se entrenaron tres modelos:

- ✅ **Regresión Logística**
- ✅ **Random Forest**
- ✅ **XGBoost**

Todos alcanzaron:

- AUC-ROC = 1.0000  
- Recall = 100.0%  
- Cumplimiento de los KPIs definidos por el negocio

## ⚠️ Observaciones

Los resultados muestran señales claras de **overfitting**, probablemente por:

- Datos limpios y poco ruidosos
- Muchas variables redundantes o con alta correlación
- Posible fuga de información

### 🔧 Posibles mejoras

- Validación cruzada más estricta  
- Reducción de dimensionalidad o selección de variables  
- Revisión de posibles variables con leakage (`EndDate`)

## 📈 Objetivo cumplido

El proyecto logró construir un modelo funcional de clasificación de churn que cumple con los requerimientos del negocio. Se recomienda fortalecer la robustez y generalización en futuras versiones.
