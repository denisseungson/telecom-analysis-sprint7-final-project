# telecom-analysis-sprint7-final-project
📊 Proyecto 6 - Análisis de Clientes de Telecomunicaciones (ConnectaTel)

📌 Descripción del Proyecto

Este proyecto tiene como objetivo analizar el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones con operaciones en Latinoamérica.

A partir de información de usuarios, planes contratados y registros de uso de llamadas y mensajes, se realizó un proceso completo de limpieza, exploración, análisis estadístico y segmentación de clientes para identificar patrones de consumo, detectar comportamientos atípicos y generar recomendaciones de negocio.

🎯 Objetivos
Analizar el comportamiento de uso de llamadas y mensajes de los clientes.
Detectar problemas de calidad de datos y corregirlos.
Identificar valores atípicos (outliers).
Segmentar clientes según edad y nivel de uso.
Generar insights que apoyen la toma de decisiones comerciales.
Proponer mejoras en la oferta de planes y estrategias de retención.

📂 Datasets Utilizados
plans.csv

Contiene información sobre los planes ofrecidos por la empresa:

plan
precio mensual
minutos incluidos
GB incluidos
costo por consumo adicional
users_latam.csv

Información de los clientes:

user_id
age
city
reg_date
plan
churn
usage.csv

Registros de actividad de los usuarios:

id
user_id
type (call o text)
duration
length
date

🔎 Etapas del Análisis
1. Carga y Exploración de Datos
Importación de librerías.
Carga de datasets.
Revisión de estructura, dimensiones y tipos de datos.
2. Calidad de Datos
Identificación de valores nulos.
Detección de sentinels e inconsistencias.
Validación de variables categóricas.
Revisión de fechas fuera de rango.
3. Limpieza de Datos
Reemplazo del valor sentinel -999 en edad.
Sustitución del valor "?" por valores nulos.
Corrección de fechas futuras.
Validación de nulos dependientes del tipo de registro.
4. Análisis Estadístico
Estadísticas descriptivas.
Distribuciones de variables numéricas.
Frecuencias de variables categóricas.
5. Detección de Outliers
Histogramas.
Boxplots.
Método IQR para validación de valores extremos.
6. Segmentación de Clientes
Segmentación por nivel de uso:
Bajo uso
Uso medio
Alto uso
Segmentación por edad:
Joven
Adulto
Adulto Mayor
7. Insights de Negocio
Identificación de segmentos de mayor valor.
Detección de oportunidades comerciales.
Recomendaciones para optimizar la oferta de planes.

🛠️ Tecnologías Utilizadas
Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook
GitHub

▶️ Cómo Ejecutar el Proyecto
Opción 1: Google Colab
Descargar el archivo .ipynb.
Abrir Google Colab.
Seleccionar Archivo → Subir Notebook.
Cargar el notebook.
Ejecutar las celdas en orden.
Opción 2: Jupyter Notebook
Clonar el repositorio:
git clone URL_DEL_REPOSITORIO
Entrar al proyecto:
cd telecom-analysis
Instalar dependencias:
pip install pandas numpy matplotlib seaborn jupyter
Ejecutar:
jupyter notebook
Abrir el notebook principal y ejecutar todas las celdas.

🔄 Guía de Reproducción
Descargar o clonar este repositorio.
Colocar los archivos:
plans.csv
users_latam.csv
usage.csv
Abrir el notebook.
Ejecutar las celdas en orden desde el inicio.
Revisar las visualizaciones, estadísticas y conclusiones generadas.

💡 Principales Hallazgos
Se identificaron problemas de calidad de datos relacionados con sentinels y fechas fuera de rango.
Los usuarios de alto consumo representan el segmento de mayor valor para la empresa.
Se detectaron patrones de uso intensivo que justifican ofertas diferenciadas.
La segmentación por edad y comportamiento permite diseñar estrategias comerciales más efectivas.

👩‍💻 Autor

Denisse Ungson

Proyecto desarrollado como parte del Bootcamp de Análisis de Datos, Sprint 7.
