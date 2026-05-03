# Ajustes globales en física de partículas

Este repositorio contiene el código fuente, los datos y los gráficos desarrollados para mi Trabajo de Fin de Grado (TFG) en Física en la Universidad Europea de Valencia (Curso 2025-2026).

## Descripción del Proyecto
El proyecto compara la inferencia estadística clásica utilizando el paquete `flavio` con un modelo de Inteligencia Artificial basado en Procesos Gaussianos para optimizar ajustes globales en física del sabor ($b \rightarrow s \ell \ell$).

## Estructura del Repositorio
* `Codigo_flavio/`: Scripts y Jupyter Notebooks con los ajustes 1D, 2D y 4D usando inferencia tradicional (MINUIT).
* `Codigo_ML/`: Implementación del emulador basado en Procesos Gaussianos.
* `Plots/`: Contornos de verosimilitud y gráficas generadas por los distintos códigos.
* `Modelos_IA/`: Archivos `.joblib` con los modelos pre-entrenados listos.

## Requisitos y Dependencias
Para ejecutar los notebooks y reproducir los resultados, se requiere **Python 3** y las siguientes librerías de terceros:

**Física Fenomenológica y Minimización:**
* `flavio` y `wilson` (Cálculo de observables teóricos y coeficientes de WET)
* `iminuit` (Minimización y estimación asimétrica de errores)

**Cálculo Científico y Análisis de Datos:**
* `numpy` y `pandas` (Manejo de matrices y estructuras de datos)
* `scipy` (Muestreo por Hipercubo Latino `qmc`, optimización, interpolación y álgebra lineal)
* `numdifftools` (Diferenciación numérica)

**Machine Learning:**
* `scikit-learn` (Procesos Gaussianos, algoritmo K-Means y escalado)
* `joblib` (Exportación y carga de los emuladores de IA)

**Visualización:**
* `matplotlib` (Gráficas de contornos y perfiles de verosimilitud)
* `corner` (Generación de corner plots multidimensionales)

## Modelos Pre-entrenados
Debido a las limitaciones de tamaño de archivo de GitHub, los modelos pre-entrenados más grandes (.joblib) están alojados externamente:
* Descargar Emulador 2D (141MB)(https://drive.google.com/file/d/1sOR-yjZrL714-swZ-eDaNLdwFVuDl0ey/view?usp=sharing)
* Descargar Emulador 4D (3GB)(https://drive.google.com/file/d/1wyfDec7T3sHMMy85itDAuhJ1Mm_jvffB/view?usp=sharing)
* Descargar Emulador 6D (3GB)(https://drive.google.com/file/d/1INGvyDBTy7-hFaMC37Wy5EUxyj_tTlW4/view?usp=sharing)

Para utilizar el notebook de ML, descarga los modelos y colócalos en la carpeta `Modelos_IA/`.

## Declaración de Transparencia y Uso de IA
En cumplimiento con la normativa de la universidad para el desarrollo del TFG:
* **Uso de IA:** Se ha utilizado Gemini como herramienta de asistencia para la estructuración de visualizaciones con Matplotlib. El diseño de la arquitectura y la lógica fenomenológica son de autoría propia. 

## Autor
* **Alberto Molina Cruz** - Grado en Física
* **Tutor:** Hector Gisbert Mullor
