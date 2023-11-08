# PI_02_AccesoInternet.

### **Rol a desarrollar**

Una empresa prestadora de servicios de telecomunicaciones nos encarga la realización de un **análisis** completo que permita reconocer el comportamiento de este sector a nivel nacional. Considerando que la principal actividad de la empresa es brindar **acceso a internet**, pero también es importante considerar el comportamiento asociado al resto de los servicios de comunicación, con el fin de orientar a la empresa en brindar una buena calidad de sus servicios, identificar oportunidades de crecimiento y poder plantear soluciones personalizadas a sus posibles clientes.

`KPIs`

Graficar y medir el KPI en un dashboard. Y graficar un segundo KPI que consideres relevante para la temática. 
El KPI propuesto es:
- *Aumentar en un 2% el acceso al servicio de internet para el próximo trimestre, cada 100 hogares, por provincia*.
La fórmula es la siguiente:

 $`KPI = ((Nuevo acceso - Acceso actual) / Acceso actual) * 100`$
 
Donde:

- "Nuevo acceso" se refiere al número de hogares con acceso a Internet después del próximo trimestre.
- "Acceso actual" se refiere al número de hogares con acceso a Internet en el trimestre actual.

# <h1 align="center">**`Autor:` Juan Ramón Perales Sosa.**</h1>

![internetNube](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/06a43cb1-e90c-4ed7-b769-8462204885ec)

  
# <h1 align="center">**Estructura de trabajo para realizar el trabajo solicitado por la empresa de Telecumunicaciones.**</h1>

![estructura](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/8467f7b8-4d00-45ab-9e39-84783e8c66dc)

  
## ETL.
### Importación de Librerias.
### Cargando la URL y opteniendo respuesta del requests.
### Instanciando reponse para leer el contenido del archivo en memoria como una cadena de texto.
### Creando un DataFrame df con las instantancias anteriores y viendo su contenido.
### Guardando los resulatdos en un archivo csv.
### Instanciando para crear un nuevo DataFrame con el archivo creado en csv.
### Observando el dimencionamineto del DataFrame.
### Diccionario del DataFrame.
### Analizamos los distintos tipos de datos por columna.
### Información del DataFrame.
### Descripción del DataFrame.
### Observando valores únicos en la columna Provincia.
### Cambiando valores no entendibles de la columna Provincia, por valores legibles.
### Observando cuantos ceros por columnas.
### Observando como quedo el DataFrame.
### Guardando DataFrame en un .parquet
### Creando DataFrame con el archivo parquet.
### Almacenando la instancia que contiene mi DataFrame.
### Liberando Memoria.

## EDA.
### Importando Librerias.
### Importando DataFrame.
### Ver si hay valores duplicados.
### Medidas descriptivas.
* Obteniendo la cantidad de valores Nulos en cada columna.
* Mostrando como se va visualizando mi DataFrame.
* Obteniendo la descrición estadistica del DataFrame.
### Mostrando cantidad de valores nulos por columna.
### Mostrando el porcentaje de valores nulos.
### Dimencion del DataFrame.
### Descripción del DataFrame.
### Histogramas.
* Reaizamos un Histograma con las siguientes columnas: 'BandAnchaFija', 'Dial_up', 'ADSL', 'Cablemodem', 'FibraOptica', 'Wireless', 'OtrosTipoConexión', 'totalServicios'.
  * Todas las distribuciones presentan un gran sesgo a la derecha.

![histograma](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/01c868e0-8e4b-472b-8f88-3a16783d57aa)

### Outliers.
* Graficamos las siguientes variables que podemos utilizar (ya que no tienen valores nulos).
* Filtramos outliers de crew_aboard.
* Criterio de selección.
* Filtramos outliers de crew_fatalities.
* Criterio de selección crew_fatalities.
* Criterio de selección, si crew_aboard > crew.fatalities.

![outliers1](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/7440246b-3567-434d-8342-df27ef7e46aa)

  
### Gráficos de barras.

![metrica2](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/8a3c5d7f-5b75-4ba1-b67a-e97582b32216)


## Metricas.

![metrica1](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/3f8a923e-fcc8-44a5-90f3-b1ad672336d5)

![pastel](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/d09b557a-0c52-4e96-baec-56757b7ecb6c)

## KPIs.
### Importando Librerias.
### Importando DataFrame.
### Seleccionando Columnas par mi nuevo DataFrame.
### Calcula el 'nuevoAcceso' desplazando las AccesoCada100Hogares un Trimestre hacia abajo.
### Obteniendo resultado para mi KPI.
 * Aumentar en un 2% el acceso al servicio de internet para el próximo trimestre, cada 100 hogares, por provincia.

![kpi1](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/90134127-2d03-4f4e-8893-d4ede4539509)

### Segundo KPI.
 * Obteniendo los servicios que se han adquirido por provincia por cada 100 hogares.

![kpi2](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/a1b0f6e3-138b-41ab-9334-716a417c8718)

## MySQL.
### Observando DatasFrame para crear base de datos.
### Creando Base de Datos y tablas en MySQL con mis DataFrame.

![sql1](https://github.com/ingjuanrps/PI_02_AccesoInternet/assets/114045466/a129beb5-cd6c-4a4b-ac8c-1822405633f3)

`Contacto:` ing.juanrps@gmail.com





























