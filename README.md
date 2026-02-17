# TFG — Predicción de billetes (rutas y clases) con modelos supervisados y secuenciales

Este repositorio contiene el código (en forma de notebooks) utilizado en un Trabajo Fin de Grado para modelar y evaluar la predicción del siguiente billete de un usuario en dos tareas:

- **Predicción de ruta** (Origen–Destino / `ruta_id`)
- **Predicción de clase** (tipo de producto / `clase_id`)

Se comparan baselines y modelos de aprendizaje automático, evaluados con **Top-k accuracy** (Top-1, Top-2, Top-3).

> ⚠️ **Nota importante:** los datos originales **no se publican** por motivos de confidencialidad. Por ello, los notebooks **no son ejecutables** sin aportar los ficheros de datos en local.

---

## Estructura del repositorio

- `01_datos.ipynb`  
  Preparación y análisis de datos, creación de variables, mapeos (ids), y generación de artefactos intermedios necesarios para modelado.

- `02_modelos.ipynb`  
  Entrenamiento y evaluación de modelos (DNN, XGBoost, RNN) y baselines, con reporte de métricas Top-k y generación de figuras/tablas.

- `figuras/`  
  Carpeta de salida para figuras.

- `data/`  
  Carpeta esperada para los datos.

---

## Requisitos

Instala dependencias con:

```bash
pip install -r requirements.txt
