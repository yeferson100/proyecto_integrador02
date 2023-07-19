<img src=https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png><p>

# PROYECTO INTEGRADO Nro 2

## ANÁLISIS DE SERVICIO DE INTERNET EN EL TERRITORIO NACIONAL

Este proyecto presenta un análisis detallado del comportamiento del servicio de internet en Argentina desde el año 2014 hasta 2022. Se examinan aspectos clave como la cobertura del servicio, protocolos de conexión y disponibilidad del mismo.

### OBJETIVOS

- Realizar una Extracción, Transformación y Carga (ETL) de la información suministrada en el siguiente enlace: [https://www.enacom.gob.ar/](https://www.enacom.gob.ar/).
- Realizar un análisis gráfico sobre el servicio de internet en Argentina.
- Crear un Control de Mando (Dashboard).
- Medir Indicadores Clave de Rendimiento (KPI).

### Extracción de la información y EDA

En el archivo ETL-EDA.ipynb se realiza la carga, transformación y análisis preliminar de los datos. Se obtienen los siguientes conjuntos de datos desde [https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/):

- AccesosaInternetfijoporvelocidaddebajadaylocalidad_2776171689206806462.csv
- ConectividadalserviciodeInternet_2776151689206559167.csv
- historico_velocidad_internet.csv
- Denuncias_y_reclamos_202306.csv
- Internet_Accesos-por-tecnologia.csv
- Internet_Accesos-por-velocidad.csv
- Internet_BAF_nal.csv
- Internet_BAF_Prov.csv
- Internet_Ingresos.csv
- Internet_Penetracion_hab.csv
- Internet_Penetracion_Hogar.csv

#### Paso 1: Conocer los Datos

- Identificación del tamaño y tipo de cada conjunto de datos, y búsqueda de columnas con nombres en común.
- Renombrar columnas y corregir datos incorrectos.
- Creación de nuevos conjuntos de datos con datos en común y tamaños similares.
- Limpieza de datos erróneos y faltantes.
- Corrección de formatos incorrectos.

#### Paso 2: Preparar los Datos

- Cambio de formato de los datos incorrectos.
- Reemplazo de ',' por '.' y ajuste a formatos correctos.
- Organización de los nuevos conjuntos de datos para su almacenamiento en una base de datos MySQL.

#### Paso 3: Análisis Gráfico y Descriptivo

- Uso de la función `.describe()` para observar el comportamiento de los datos numéricos.
- Identificación de valores máximos, mínimos, media, desviación y distribución de los datos.
- Uso de la función `corr()` para observar las correlaciones entre los datos numéricos.
- Generación de diagramas de dispersión para visualizar la relación entre variables.
- Creación de histogramas para analizar la distribución y detectar sesgos.

#### Paso 4: Análisis de Cobertura y Calidad del Servicio de Internet

En este análisis se plantean las siguientes preguntas:

- ¿Cuántos hogares tienen acceso a internet?
- ¿Qué tipos de conexiones están disponibles?
- ¿Cuáles son las velocidades de descarga o conexión disponibles?
- ¿Cuántas provincias tienen acceso a internet y qué tipo de acceso tienen?
- ¿Cuál ha sido el crecimiento en el acceso a internet?
- ¿Cuál ha sido el crecimiento de las velocidades de conexión?
- ¿Cuál ha sido el crecimiento en las conexiones a internet?

Se desarrolla un Dashboard que muestra el comportamiento y la cobertura del servicio de internet en Argentina. El archivo del Dashboard es Proyecto2.pbx.


<hr>

## **ANALISIS**

<hr>

### **PAGINA 1**
<img src="Captura de pantalla 2023-07-18 195459.png"  height=500>


### **PAGINA 2**
 
<img src="Captura de pantalla 2023-07-18 202446.png"  height=500>



## *CONCLUSIONES OBTENIDAS*

### 1. En Argentina, la velocidad promedio de descarga actual es de 58.67 Mbps. 


### 2. La provincia con la mayor cantidad de usuarios conectados es 'Capital Federal', mientras que 'Formosa' cuenta con la menor cantidad de usuarios. 


### 3. El año 2022 registró la mayor cantidad de ingresos, alcanzando la suma de 182.981.651 pesos. 


### 4. La fibra óptica ha experimentado una tendencia alcista desde 2018 hasta 2022.


### 5. En efecto, el promedio de Mbps en Argentina ha mantenido un crecimiento constante, comenzando en 3.85 y llegando actualmente a 58.67.


### 6. La tecnología más utilizada es el 'Cable Modem', con un total de 144.291.039 instalaciones. 


### 7. Los ingresos han mostrado un crecimiento constante a lo largo de la historia, sin retrocesos.

<hr>

## *KPIS*

### 1. Creamos un KPI que nos indica si aumento o bajo la tasa de accesos a internet comparando el año actual con el año anterior 

### 2. Creamos un KPI que no mide la velocidad promedio de bajada en Mbps con un objetivo de llegar al 40 Mbps siendo cumplida en el año 2020

### 3. Creamos un KPI que nos mide el total de ingresos a lo largo de la historia(se puede filtrar por año) y como objetivo tiene llegar a 190 millones de pesos para el año proximo, faltando un monto de 7 millones de pesos para cumplir con el objetivo 


<hr>

## Descripcion de los datos utilizados

### **Año :**                          <h3 align=center>  rango años del 2014 a 2022 </h3>
### **ADSL :**                         <h3 align=center>Cantidad de instalaciones con  tecnologia ADSL </h3>
### **Cablemodem :**                   <h3 align=center>Cantidad de instalaciones con tecnologia Cablemodem </h3>
### **Fibra optica :**                 <h3 align=center>Cantidad de instalaciones con la tecnologia de Fibra optica </h3>
### **Wireless :**                     <h3 align=center>Cantidad de instalaciones con la tecnologia de Wireless </h3>
### **Mbps (Meda de bajada) :**        <h3 align=center>Velocidad promedio de bajada en Mbps </h3>
### **Provincia :**                    <h3 align=center>Provincias de Argentina </h3>
### **Accesos por cada 100 hogares :** <h3 align=center>Cantidad de hogares que tienen acceso a conexion a internet </h3>
### **KPI :**                          <h3 align=center>Nos indica si subio o bajo la tasa de 'accesos por cada 100 hogares' </h3>
### **Tasa accesos :**                 <h3 align=center>Tasa porcentual de la columna 'accesos por cada 100 hogares' </h3>
### **Ingresos(en miles de pesos) :**  <h3 align=center>Ingresos generados por la empresa </h3>

<hr>

### *Firma:* https://www.linkedin.com/in/mauro-ferrera/

#### Gracias por ver <3