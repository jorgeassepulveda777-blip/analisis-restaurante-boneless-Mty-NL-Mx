# Proyecto: Ubicación óptima para un restaurante de boneless en Monterrey, Nuevo León, México

---

## 1. Pregunta Principal del Proyecto

¿Qué zona del municipio de Monterrey presenta mayor potencial para abrir un restaurante de boneless rentable, considerando factores como:

- Afluencia de personas  
- Competencia  
- Nivel socioeconómico  

---

## 2. Justificación de la Pregunta

### 2.1 Importancia crítica de la ubicación

La ubicación es uno de los factores más determinantes para el éxito de un restaurante. Diversos análisis dentro de la industria gastronómica coinciden en que elegir un buen lugar impacta directamente en la rentabilidad y permanencia del negocio.

Sin el uso de datos, esta decisión se basa en suposiciones, lo que incrementa el riesgo operativo y financiero.  
El análisis de datos permite transformar una decisión intuitiva en una estrategia medible y fundamentada.

---

### 2.2 Justificación de los factores seleccionados

Los factores elegidos (afluencia, competencia y nivel socioeconómico) están respaldados por metodologías de análisis utilizadas en inteligencia de negocios.

La concentración geográfica de clientes y negocios permite identificar:

- Zonas con alta demanda  
- Zonas saturadas  
- Oportunidades de mercado  

---

## 3. Importancia de cada factor

### 3.1 Afluencia (demanda o flujo de personas)

El flujo de personas determina el tamaño del mercado disponible.

La mayoría de los restaurantes generan entre el 70% y 80% de sus ingresos de clientes cercanos.

Conclusión:  
Sin afluencia, no existe demanda suficiente.

---

### 3.2 Competencia

La competencia representa la cantidad de negocios similares en una zona.

- Alta competencia → menor participación de mercado  
- Baja competencia → puede indicar oportunidad o baja demanda  

Conclusión:  
A mayor competencia, menor potencial de rentabilidad.

---

### 3.3 Nivel socioeconómico

El nivel socioeconómico define la capacidad de consumo de los clientes.

Para un restaurante de boneless (segmento casual), se requieren zonas con niveles:

- Medio  
- Medio-alto  

Conclusión:  
El nivel socioeconómico determina la viabilidad económica del negocio.

---

## 4. Análisis integral

Los factores deben analizarse en conjunto:

- Alta afluencia sin ingreso → bajo consumo  
- Alto ingreso sin flujo → pocos clientes  
- Alta competencia → menor participación  

El análisis conjunto reduce el riesgo y mejora la toma de decisiones.

---

## 5. Conclusión

El uso combinado de los factores permite transformar la selección de ubicación en un proceso basado en datos.

---

## 6. Análisis de Nivel Socioeconómico (ETL)

Este proyecto incorpora datos reales de nivel socioeconómico mediante un proceso ETL.

---


## 6.1 Fuente de datos

Datos obtenidos de:

https://www.amai.org/NSE/index.php?queVeo=NSEDES  

Basados en:
- INEGI (ENIGH + Censo 2020)  
- Modelos de clasificación socioeconómica  

Nivel de detalle:
- Municipio  
- Localidad  
- AGEB  

images/FuenteNSE.png

---

## 6.2 Flujo de trabajo (ETL)

### Extract (Obtención)

Datos descargados en formato Shapefile:

- .shp → geometría  
- .dbf → atributos  
- .shx → índice  

---

### Transform (Python)

Se extrajeron los datos del archivo .dbf y se convirtieron a formato CSV utilizando Python.

images/transformadorNSE.png

Resultado:
- Conversión de DBF a CSV  
- Preparación de datos para análisis en Power BI  

---

### Load (Power BI)

El archivo CSV fue importado en Power BI para su análisis.

---

### Transform (Power BI / Power Query)

En Power BI se realizó la limpieza y transformación de datos, incluyendo:

- Eliminación de valores nulos  
- Corrección de tipos de datos  
- Estandarización de nombres  
- Selección de variables relevantes  


Resultado:
- Dataset limpio y estructurado para análisis  

---

## 7. Visualización preliminar en Power BI

Como resultado del proceso de limpieza y transformación de datos, se generaron visualizaciones iniciales para explorar el nivel socioeconómico por municipio.

### Distribución del nivel socioeconómico por municipio

images/PBI_NSE.png

Esta visualización muestra la distribución de los niveles socioeconómicos por municipio, permitiendo identificar las zonas con mayor presencia de niveles medios y altos, lo cual es clave para evaluar el potencial de consumo en el análisis de ubicación del restaurante.


