# Beyond the Title: Causal Evidence of Land Formalization on Coca, Credit, and Violence in Colombia's Peace Process Implementation

**Autor:** Daniel Ricardo Amaya Alba

Este repositorio contiene el paquete de replicación, la base de datos consolidada y el documento final del trabajo de grado. 

##  Contenido del Repositorio

En este repositorio de GitHub encontrarás los siguientes archivos principales:

* `TrabajoFinal.pdf`: Documento final compilado con los resultados y análisis.
* `TrabajoFinal.qmd`: Código fuente en Quarto utilizado para generar el documento PDF, incluyendo todas las estimaciones y análisis econometrico.
* `panel_tierras_violencia_final.csv`: Base de datos final estructurada a nivel municipal lista para la estimación de los modelos.

## ️ Instrucciones de Replicación

### 1. Replicar estimaciones y documento final
Si su objetivo es revisar o replicar los modelos econométricos y generar el PDF:
1. Clona o descarga este repositorio.
2. Abre el archivo `TrabajoFinal.qmd` en RStudio.
3. Asegúrate de tener el archivo `panel_tierras_violencia_final.csv` en la misma carpeta.
4. Ejecuta el código y renderiza el documento completo.

### 2. Replicar la construcción de la base de datos (Data Pipeline)
Si deseas reconstruir el panel principal de datos (`panel_tierras_violencia_final.csv`) desde las fuentes originales, sigue estos pasos:

1. Dirígete a la siguiente carpeta de Google Drive: [Repositorio de Bases de Datos Originales](https://drive.google.com/drive/folders/1WdurRoyh2Vh24rdbDVRblZqy7Q75WYht?usp=share_link)
2. Descarga la carpeta completa donde encontrarás: 
   * Un archivo comprimido: `RRI Formalización Construcción Base de Datos-20260529T024614Z-3-002.zip`
3. Extrae el contenido del archivo `.zip` en una carpeta de tu computadora.
5. Abre el script `contruyendo_panel_tierras_violencia_final.R`.
6. **Paso fundamental:** Define el *Working Directory*  en esa carpeta. En RStudio ve a: `Session` > `Set Working Directory` y escoge como directorio la carpeta que descargaste.  
7. Corre todo el script. Al finalizar, el panel consolidado se exportará automáticamente en esa misma carpeta.

##  Declaración de uso de Inteligencia Artificial

Para el desarrollo de este trabajo se utilizó asistencia de IA como herramienta de apoyo, bajo supervisión humana, en las siguientes tareas:

* **Gemini:** Asistencia en la estructuración de formato, ajuste de tablas con libreria kableextra y configuración de hipervínculos en el archivo `.qmd` para garantizar la correcta compilación y renderizado del documento PDF.
* **GitHub Copilot:** Automatización de procesos de escritura repetitivos en RStudio (ej. adaptación de código para múltiples especificaciones de un mismo modelo econométrico). Todas las sugerencias fueron auditadas y verificadas manualmente por el autor para garantizar la precisión analítica.
* **Claude Code:** Verificación de la estructura y el ensamblaje del panel de datos municipal, siguiendo los estándares y recomendaciones de control de calidad metodológica expuestos por Scott Cunningham en su blog personal.