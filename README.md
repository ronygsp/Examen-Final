# Análisis de Churn para Interconnect Telecomunicaciones

## Descripción

Este proyecto implementa un análisis completo de predicción de churn (abandono de clientes) para Interconnect, una empresa de telecomunicaciones. Siguiendo la metodología CRISP-DM, se desarrollaron modelos de machine learning para identificar clientes con probabilidad de abandonar los servicios y proponer estrategias de retención optimizadas.

## Estructura del Proyecto

- **notebooks/**: Contiene el notebook principal del análisis
  - `Salgado_Ronald_churn.ipynb`: Notebook principal con el análisis completo
- **data/**: Directorio con los datos utilizados (no incluido en el repositorio)
  - `contract.csv`: Información sobre los contratos de clientes
  - `personal.csv`: Datos personales de los clientes
  - `internet.csv`: Detalles de servicios de internet
  - `phone.csv`: Información de servicios telefónicos
  - `processed_data.pkl`: Datos procesados para modelado

## Metodología CRISP-DM

El proyecto sigue las seis fases de la metodología CRISP-DM:

1. **Comprensión del Negocio**: Definición de objetivos y KPIs
2. **Comprensión de los Datos**: Exploración de fuentes de datos y distribuciones
3. **Preparación de los Datos**: Limpieza, transformación y creación de features
4. **Modelado**: Implementación de modelos de predicción (Regresión Logística, Random Forest, XGBoost)
5. **Evaluación**: Comparación de modelos según AUC-ROC y Recall
6. **Despliegue**: Plan de integración, monitoreo y estrategias de retención

## Resultados Clave

- Se implementaron tres modelos supervisados con diferentes enfoques algorítmicos
- Se logró un rendimiento de AUC-ROC superior a 0.85 y Recall superior a 80%
- Se desarrolló una estrategia de descuentos segmentada por valor de cliente y probabilidad de abandono

## Requisitos

- Python 3.8+
- Pandas, NumPy, Scikit-learn
- Matplotlib, Seaborn
- XGBoost
- Jupyter Notebook

## Uso

1. Clone este repositorio
2. Coloque los archivos de datos en la carpeta `data/`
3. Ejecute el notebook `Salgado_Ronald_churn.ipynb` para reproducir el análisis completo

## Autor

Ronald Salgado - Universidad San Francisco de Quito
