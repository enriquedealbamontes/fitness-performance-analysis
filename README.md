# Gym Members Exercise Tracking Analysis

### 1) Objetivo
- Analizar datos de entrenamiento físico para estudiar la relación entre duración de entrenamiento, calorías quemadas e indicadores físicos.

### 2) Dataset
- Fuente: Gym Members Exercise Tracking Dataset
- Variables clave: calorías quemadas, duración del entrenamiento, género, altura, peso y tipo de entrenamiento.

### 3) Preguntas
- ¿Existe relación entre duración y calorías?
- ¿Cómo afecta el IMC?
- ¿Existen diferencias entre tipos de entrenamiento?

### 4) Data issues & fixes
- Valores duplicados eliminados mediante funciones de limpieza.
- Conversión y tratamiento de variables numéricas.
- Creación de nuevas variables derivadas para mejorar el análisis.

### 5) Pipeline
- raw → clean → features → viz → export

### 6) Hallazgos
- Insight 1: A mayor duración del entrenamiento, mayor gasto calórico.
- Insight 2: El IMC permite comparar distintos perfiles físicos.
- Insight 3: Las visualizaciones muestran correlaciones entre variables numéricas.

### 7) Estructura del proyecto
- `src/` contiene funciones reutilizables (`cleaning`, `features`, `viz`)
- `main.py` ejecuta el pipeline end-to-end
- `notebooks/eda.ipynb` contiene el análisis y visualizaciones

### 8) Cómo ejecutar
- `pip install -r requirements.txt`
- Ejecutar pipeline: `python main.py`
- Abrir notebook: `notebooks/eda.ipynb`

## Estructura recomendada del proyecto

```text
project/
├── main.py
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   └── eda.ipynb
├── src/
│   ├── __init__.py
│   ├── cleaning.py
│   ├── features.py
│   ├── viz.py
├── README.md
├── requirements.txt
```

```