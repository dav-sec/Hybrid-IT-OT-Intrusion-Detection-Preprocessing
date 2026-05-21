# Hybrid IT/OT Intrusion Detection Preprocessing

## Descripción

Este proyecto implementa un pipeline completo de preprocesamiento de datos para sistemas de detección de intrusiones (IDS) en entornos híbridos IT/OT e IoT utilizando técnicas de Machine Learning.

El pipeline integra tráfico de red y logs de dispositivos para generar datasets optimizados y listos para entrenamiento de modelos de inteligencia artificial.

---

# Objetivos

- Limpiar y normalizar datasets IT/OT
- Fusionar tráfico de red y logs IoT
- Transformar variables categóricas y numéricas
- Balancear clases mediante SMOTE
- Reducir dimensionalidad utilizando PCA
- Generar datasets optimizados para modelos ML/DL

---

# Pipeline del Proyecto

## Fase 1 — Limpieza de Datos
- Eliminación de valores nulos
- Eliminación de duplicados
- Corrección de tipos de datos
- Normalización básica

### Output
```text
clean_flows.csv
clean_logs.csv
```

---

## Fase 2 — Fusión IT/OT
- Sincronización temporal
- Integración de tráfico y logs
- Construcción del dataset híbrido

### Output
```text
fused_it_ot.csv
```

---

## Fase 3 — Transformación
- Label Encoding
- Z-Score Standardization
- Extracción temporal
- Conversión de variables categóricas

### Output
```text
transformed_it_ot.csv
```

---

## Fase 4 — Balanceo y Reducción
- Balanceo de clases con SMOTE
- Reducción dimensional mediante PCA
- Conservación de >99% de varianza

### Outputs
```text
balanced_it_ot.csv
reduced_it_ot.csv
```

---

# Dataset Final

El dataset final optimizado es:

```text
reduced_it_ot.csv
```

Características:
- Balanceado
- Escalado
- Reducido dimensionalmente
- Optimizado para ML/DL

---

# Tecnologías Utilizadas

- Python 3
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
- Joblib

---

# Modelos Compatibles

El dataset generado está preparado para:

- XGBoost
- LightGBM
- Random Forest
- Deep Neural Networks (DNN)
- Stacking Ensemble

---

# Estructura del Proyecto

```text
├── input/
├── output_phase1/
├── output_phase2/
├── output_phase3/
├── output_phase4/
├── notebooks/
├── models/
└── README.md
```

---

# Resultados del Preprocesamiento

## Dataset Original
- 3,907,536 registros

## Dataset Balanceado
- 7,644,154 registros

## PCA
- 10 componentes principales
- >99.99% de varianza explicada

---

# Autor

Proyecto desarrollado para investigación en ciberseguridad e IDS híbridos IT/OT utilizando Inteligencia Artificial.

---

# Licencia

MIT License
