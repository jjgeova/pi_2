# PROYECTO INDIVIDUAL 2

## Temática: Data Analytics


### Analizar la data desde sus fuentes de datos y realizar analisis en EDA para luego presentar en Power BI y otro los KPI con sus recomendaciones para la empresa.

Proyecto de ciencia de datos para las fuentes de información en formato de Excel .xlsx con columnas. Para lo cual se deben aplicar las técnicas necesarias para procesar la información y mejorar la calidad de los datos en primera instancia, siendo el objetivo principal el analisis desde el EDA y la presentacion de informacion. 

Para esto, es necesario realizar el proceso de **ETL** (Extracción, Transformación y Carga) sencillo, en el cual se lleva a cabo una comprensión estructural y de la información de los datos. Después de ello, sigue el **EDA** (Análisis Exploratorio de Datos), donde se realiza un análisis de la información luego de ser transformada y depurada.

El proyecto requiere la creación de **KPIs** para mostrar los indicadores de gestion en sus objetivos propuestos en cada trimestre, año o provincia.

---

## Origen de los Datos

Los archivos de datos se encuentran en formato **xlsx**. El primero de ellos, llamado `internet`, que contiene **15 hojas** cada una con un numero determinado de filas y columna, la informacion esta segmentada dando la posibilidad de unir varias hojas en una sola base de datos, esto siempre y cuando existan campos de referencia de igual tipo.

---

## Limpieza y Transformación de los Datos (ETL)

En este proceso se analizó la estructura de los datos y su contenido de manera minuciosa, encontrando variedad de tipos de datos, aunque distribuidos en varias hojas del archivo de excel.

De acuerdo con los requerimientos del proyecto, se abordaron los siguientes pasos:

1. **Depuración de datos nulos**: Se listaron las cantidades de datos nulos por cada campo, y se procedió a depurarlos hasta lograr que ningún campo contenga valores nulos.
2. **Imputación de valores numéricos**: Los valores numéricos nulos fueron reemplazados por ceros.
3. **Formateo de datos**: Se aseguraron de que los datos estuvieran correctamente formateados (por ejemplo, `date`, `float`, `int`, etc.).
4. **Unificacion de hojas en una sola data**: se logro realizar el merge desde python para velicidad por provincia, accesos por tecnologia, accesos por cada 100 hogares y accesos pro cada 100 habitantes, quedando una sola data con la informacion que denominamos "8_Penetracion_PH_AT_VP.xlsx", quedando con 927 registros y 12 columnas en total. 
Año,Trimestre,Provincia,Accesos por cada 100 hab,Accesos por cada 100 hogares,ADSL,Cablemodem,Fibra óptica,Wireless,,Otros,Total Y	Mbps (Media de bajada).


### Consideracion 

Llevamos la informacion al diseñador de Dasboard organizada desde Python, para evitar hacer transformaciones por ejemplo en la herramienta de Power BI, de esta menera facilitamos el diseño.

---

## Análisis Exploratorio de los Datos (EDA)

Durante este análisis, se observaron varias características de los datos, tales como:

- Velociades (Mbps) de internet bajas, medianas y altas en el territorio de Argentina.
- Accesos a internet por cada 100 hogares.
- Accesos a internet por cada 100 habitantes.
- Accesos por tecnologia.

Caracteristicas relacionados con alguna provincia de Argentina, año y trimestre donde se tomo la informacion.

---

## Analisis de los datos

En terminos generales, no fue necesario un ETL profundo lo que facilita su analisis, no se encontraros outlier fuera de lo real y consistente con el servicio de internet como canal de telecomunicaciones, muy pocos valores nulos y otros en negativo.

Se realizo analisis usando ademas graficos en el EDA como:
**Gráfico de Dispersión (Scatter Plot)**
**Histograma**
**Boxplot (Gráfico de Caja)**
**Gráfico de Densidad (KDE - Kernel Density Estimate)**
**Gráfico de Barras y Lineas**

---

## Datos importantes para la toma de desiciones


1. ****:
   - **Velocidades por provincia**: No es lo mismo navegar a 10 Mbps que a 100 Mbps o mas, tambien influye la tecnologia pues se puede tener buen ancho de banda pero con tecnoligia de conexion cerca al fin de su vida util, es como tener fibra optica hasta la puerta del hogar y hacia adentro conectarse con DSL.

2. **Acceso a internet por cada 100 hogares**:
   - **Descripción**: Se sentra en el acceso y uso de internet en los hogares Argentinos, bien sabemos que esta conexion es usada frecuentemente por todos los integrantes del hogar.

3. **Acceso a internet por cada 100 habitantes**:
   - **Descripción**: Este es diferente al anterior, pues, el uso de los Smartphone facilitan la conexion a internet casi que de manera individual.
   
---

## Conclusiones

La informacion suministrada por la empresa, ofrece la informacion necesaria para determinar la necesidad de hacer alianzas publico-privadas y disminuir la brecha de acceso y tecnologia existentes en provincias con poca poblacion y alejadas de las ciudades grandes o intermedias, la empresa desde sus recursos puede aportar para la actualizacion de tecnologia y aumentar el ancho de banda de sus canales de servicio en las poblaciones donde el mismo consumo y sus ganancias permite realizarlo, en las otras poblaciones no es posible pues la tecnologia cuesta y su mantenimiento igual.

## Recomandacon
Realizar alianzas publico-privadas, bien sean ONGs internacionales, instituciones publicas, y por supuesto el sector privado, para aumentar la cobertura con tecnologia y llevar servicios a todos los rincones del Pais, el acceso a la internet de buena velocidad de carga y descarga de informacion ya no es un lujo, es una necesidad que es transversal a todas las actividades del ser humano para su beneficio y progreso social y economico, pues quien tenga mas y mejores herramientas podra competir facilmente.


## Herramientas Tecnológicas

- **Python**.
- **Power BI**.
- **GitHub**.


