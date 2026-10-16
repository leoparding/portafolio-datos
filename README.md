# Limpieza y transformación de datos de inflación e índice de precios para Tableau

**Problema:** Los archivos originales de inflación e índice de precios venían en formato ancho (un año por columna) y con valores nulos, lo que dificultaba analizarlos y visualizarlos en Tableau.
El objetivo fue transformarlos a un formato limpio, con un registro por país y año.

**Datos:** Archivos de Excel de inflación e índice de precios por país y año, suministrados en una actividad académica de la universidad (fuente original no especificada).

**Herramientas:** Python, Pandas, Google Colab, Excel, Tableau

**Qué hice:**
- Leí los archivos Excel y estandaricé los nombres de columnas (quité espacios y columnas innecesarias).
- Transformé los datos de formato ancho a largo con melt, creando las columnas País, Código de país, Año y Valor.
- Convertí los tipos de datos (año y valores a numérico) y eliminé los registros con valores nulos.
- Exporté dos archivos limpios (inflacion_limpia.xlsx e indice_limpio.xlsx) listos para conectar a Tableau.

**Resultado:** Dos datasets limpios en formato largo (un registro por país y año), sin valores nulos y listos para conectar a Tableau. 

**Enlace:** Notebook en Colab: https://drive.google.com/file/d/1QowYHS4ujIUTl41kDX2RGsia84tL135B/view?usp=sharing 
Dashboard en Tableau Public: https://public.tableau.com/views/AnalisisMundial/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
