<img width="1134" height="258" alt="image" src="https://github.com/user-attachments/assets/51c6ea08-5dd9-49f1-8fd9-df322d99a971" />

# 📈 Segundo Proyecto de Análisis de Datos: Comparación de la eficacia de distintos métodos de Regresión al predecir el peso de diferentes especies de pescado

¡Bienvenido a mi segundo proyecto de datos con Python! Este proyecto es mi primera vez implementando modelos de machine learning simples como las regresiones.

---

## 🎯 Objetivo del proyecto

El proyecto se centra en predecir el **peso de los peces** a partir de distintas medidas morfológicas **(longitudes, alto, ancho, etc.).** mediante un modelo de regresión exponencial y otro de regresión polinomial para después comprobar cual funciona mejor.

--- 

## 🐟 Variables Estudiadas

### 🎯 Variable Objetivo
**`Weight`** - Peso del pez (variable dependiente)

### 📏 Variables Predictoras
**Medidas de longitud:**
- `Length1` 📏
- `Length2` 📐  
- `Length3` 📊

**Otras dimensiones:**
- `Height` 📏
- `Width` 📐

**Especie:** `Species` 🏷️

### 🐠 Especies (7 tipos)
`PERCH` • `BREAM` • `ROACH` • `PIKE` • `SMELT` • `PARKKI` • `WHITEFISH`

---

## 🤖 Modelos comparados y métricas 
Se evaluaron dos enfoques principales: 
1. **Modelo exponencial:** aplicando una transformación logarítmica al objetivo y regresión lineal. 
2. **Modelo polinomial:** utilizando una transformación polinómica de grado 2 combinada con regresión lineal. Las métricas utilizadas para comparar el desempeño fueron: **MAE, MSE, RMSE y R²**, evaluadas sobre conjuntos de entrenamiento y prueba. Además, se analizaron los **residuales** (residuales vs. predicción, histograma y gráfico Q–Q) para validar los supuestos de los modelos.

--- 

## 🏆 Resultado principal 
El **modelo polinomial de grado 2** obtuvo un mejor desempeño en las métricas de evaluación y presentó un comportamiento de residuales más estable y sin sesgos sistemáticos. Por ello, se seleccionó como **modelo definitivo**. 

--- 

## 💾 Entrenamiento final y guardado 
El modelo polinomial se reentrenó utilizando **todos los datos disponibles** y se exportó para su uso futuro: - 📦 Modelo: fish_weight_prediction_poly_model.joblib - ⚙️ Transformador (PolynomialFeatures): final_converter.joblib 

--- 

## ⚠️ Limitaciones y recomendaciones futuras 
- **Validación:** aplicar validación cruzada y búsqueda de hiperparámetros para asegurar robustez. 
- **Regularización:** probar técnicas como Ridge o Lasso si los coeficientes muestran inestabilidad. 
- **Ingeniería de variables:** considerar la reincorporación o transformación de la variable Species y la creación de nuevas variables derivadas. - **Evaluación externa:** probar con **nuevos conjuntos de datos** para medir la capacidad de generalización. 
- **Incertidumbre:** calcular intervalos de predicción y analizar errores por subgrupos (por especie, tamaño, etc.). 
- **Producción:** desplegar el modelo mediante una API ligera (Flask/FastAPI) y establecer **pipelines de monitoreo** para detectar degradación o drift de datos.

--- 

### ✅ Conclusión general 
El análisis demuestra que  el **modelo polinomial de grado 2** logra capturar eficazmente la relación entre las medidas morfológicas y el peso de los peces. El modelo final está **entrenado, validado y exportado**, y las recomendaciones propuestas permitirán **reforzar su fiabilidad y preparación para un entorno de producción**.
