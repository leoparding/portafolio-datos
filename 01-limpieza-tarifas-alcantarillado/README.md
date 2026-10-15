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

## Visualizaciones
Registros por año y tipo de uso
<img width="1185" height="484" alt="image" src="https://github.com/user-attachments/assets/421334b1-eb89-401e-b473-5acb7fa1ce89" />

Evolución de la tarifa básica promedio
<img width="984" height="484" alt="image" src="https://github.com/user-attachments/assets/aa22eb72-1237-41b4-abbd-42d068012ff0" />

Tarifa básica por estrato (residencial).
<img width="984" height="484" alt="image" src="https://github.com/user-attachments/assets/43c4a471-1020-4d09-aeb5-dbb26efb16e5" />

Comparación de tarifas por tipo de uso 
<img width="1185" height="484" alt="image" src="https://github.com/user-attachments/assets/e6c9aa41-6ae6-495c-a0d6-82aa4426bf83" />

Mapa de calor de correlaciones

<img width="668" height="584" alt="image" src="https://github.com/user-attachments/assets/6cdce6a0-a805-4f26-aa5c-c93c67b32f56" />

 
