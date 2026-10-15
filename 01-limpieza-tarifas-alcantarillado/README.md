# Limpieza y análisis de tarifas de alcantarillado (2020–2026)

**Problema:** El dataset original tenía formatos que impedían analizarlo (años como "2,022", tarifas como texto con separador de miles, 
códigos de uso sin descripción). El objetivo fue dejarlo limpio y listo para análisis y visualización en Power BI.

**Datos:** fuente de datos https://www.datos.gov.co

**Herramientas:** Python, Pandas, NumPy, Matplotlib, Seaborn, Google Colab

**Qué hice:**
- Perfilé el dataset (tipos, nulos, duplicados, valores únicos) y trabajé sobre una copia para conservar el original.
- Corregí tipos de datos: año con coma a entero y tarifas con separador de miles a numérico.
- Creé columnas derivadas (tipo de uso descriptivo y fecha para series de tiempo), renombré y reordené columnas y exporté un CSV limpio.
- Elaboré 5 visualizaciones: registros por año y uso, evolución de la tarifa básica, tarifa por estrato (residencial),
  comparación de tarifas por uso y mapa de calor de correlaciones.

**Resultado:** Dataset limpio (Tarifas_Alcantarillado_Limpio.csv) y 5 gráficas. La tarifa básica promedio de alcantarillado muestra una 
tendencia ascendente, con su mayor salto entre 2022 y 2023, cuando pasa de $846 a $1.872 (aprox. +121%). En uso residencial, la tarifa básica 
promedio por estrato va de aprox. $1.000 a $1.750. Al comparar por tipo de uso (comercial, industrial, oficial y residencial), la tarifa fija 
se diferencia de las demás por sus valores promedio más altos, mientras que las tarifas básica, complementaria y suntuaria se mantienen en 
rangos más bajos y de comportamiento similar. El mapa de calor confirma que estas tres últimas están casi perfectamente correlacionadas 
entre sí (1.00), mientras que la tarifa fija tiene una correlación moderada con ellas (0.58).

**Enlace:** Notebook en Colab: https://colab.research.google.com/drive/1ol0T0xpmv-6m0lfwg8TjIiVAtG4wTf6y?usp=sharing

**PowerBI**: https://unadvirtualedu-my.sharepoint.com/:u:/g/personal/cfoyolac_unadvirtual_edu_co/IQBdTii6qG_-QJ_dPIYoXgvOAR7YEtxA_tofGt5ZQ3EcKDI?e=asywWJ 

<img width="700" height="438" alt="images (1)" src="https://github.com/user-attachments/assets/5e88c783-de15-46eb-9818-ac74f1328207" />

