
![image](https://github.com/user-attachments/assets/b51b7742-e4ca-41a1-ba21-c89b6b0e0fd3)

# 📈 Primer Proyecto de Análisis de Datos:  Analisis de Datos Históricos de consumo y precio en España (2000 - 2024)

¡Bienvenido a mi primer proyecto de análisis de datos con Python! Este proyecto es mi punto de partida antes de empezar a implementar ciencia de datos y machine learning en siguientes proyectos.   
En este trabajo analizamos la evolución histórica del **consumo per cápita** y del **precio** de 9 alimentos consumidos en España entre los años 2000 y 2023.

---

## 🥫 Alimentos analizados

A lo largo del proyecto, estudiaremos estos **9 alimentos** representativos de la dieta en España:

- 🥩 *CARNE DE VACUNO*
- 🍗 *CARNE DE POLLO*
- 🐖 *CARNE DE CERDO*
- 🌳 *ACEITE DE OLIVA*
- 🍅 *TOMATES*
- 🐟 *SALMÓN*
- 🍚 *ARROZ*
- 🥫 *CONSERVAS (Platos preparados en conserva)*
- 🍞 *PAN*

---

## 🎯 Objetivo del proyecto

Estudiar la relación entre dos variables clave:

- El **consumo per cápita** anual de cada alimento.
- La evolución de su **precio medio por kilogramo**.

Además, en la última parte del análisis, comparamos esta evolución con la del **salario medio anual** en España, para estudiar si el aumento del poder adquisitivo ha seguido el mismo ritmo que el encarecimiento de los alimentos.

---

## 🧰 Herramientas y librerías utilizadas

Este proyecto fue desarrollado con Python, utilizando los siguientes paquetes:

```python
from pathlib import Path
import openpyxl
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## Estructura del repositorio
```
consumo_precios_alimentos_espana/
├── Raw Data/ # Datos crudos
├── Notebooks/ # Jupyter Notebooks
├── Filtered Data/ #Datos procesados
├── requirements.txt # Dependencias del proyecto
└── README.md # Documentación del proyecto
```
---

## ¿Qué encontrarás en los notebooks?

Cada uno de los dos notebooks representa una fase distinta del análisis e incluyen:

- 📌 Limpieza y unificación de datos provenientes del Ministerio de Agricultura y Pesca de España.
- 📈 Análisis de la evolución histórica de precios y consumo per cápita desde el año 2000 hasta 2024.
- 📉 Cálculo de variaciones porcentuales, acumuladas y comparación con el salario medio(2008-2023).
- 📊 Visualizaciones gráficas de todas las tendencias relevantes.
- 📎 Observaciones y anotaciones sobre inconsistencias en los datos oficiales.

---

## Conclusiones principales

- El aumento en el precio de algunos alimentos como el *aceite de oliva* ha superado con creces la subida del salario medio.
- El consumo de algunos productos ha disminuido de forma preocupante, posiblemente por razones económicas.
- Se observa un desacoplamiento entre salario medio y coste alimentario en varios periodos.
- Los datos del año 2024 presentan anomalías debidas a un cambio metodológico en la medición por parte del Ministerio, por lo que se han descartado del análisis final.

---

## Lecciones aprendidas durante este proyecto:

- Importancia de entender el origen y la estructura de los datos antes de analizarlos.
- Gestión de inconsistencias y duplicados en datasets reales.
- Uso práctico de `pandas`, `seaborn` y `matplotlib` en análisis exploratorio.
- Subida y documentación de proyectos en GitHub de forma clara y profesional.
