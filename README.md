
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
- 🫒 *ACEITE DE OLIVA*
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
