#  Evaluaciones Agropecuarias Municipales (EVA) — Análisis Departamental

Este Jupyter Book presenta un análisis exploratorio y cartográfico de las **Evaluaciones Agropecuarias Municipales (EVA)** de Colombia, integradas con el shapefile oficial de departamentos (`MGN2023_DPTO_POLITICO`).  

El objetivo principal es **visualizar la información agrícola a nivel departamental**, permitiendo identificar patrones regionales de superficie sembrada, cosechada, producción y rendimiento.



##  Objetivos

1. **Procesar y limpiar los datos** del archivo CSV de EVA (2006–2025).  
2. **Estandarizar nombres y códigos departamentales**, asegurando correspondencia con la cartografía oficial.  
3. **Construir indicadores agregados** (suma o promedio) a nivel departamental.  
4. **Visualizar los resultados en mapas coropléticos**, resaltando las diferencias regionales.  
5. **Exportar resultados** en formatos abiertos (GeoJSON, CSV) para su reutilización en otras herramientas.


##  Fuentes de datos

- **CSV EVA**: Evaluaciones Agropecuarias Municipales del Ministerio de Agricultura.  
- **Shapefile MGN 2023**: Marco Geoestadístico Nacional (DANE), división político-administrativa de Colombia.  



##  Metodología

1. **Lectura de datos** con `pandas` y `geopandas`.  
2. **Normalización de texto** (departamentos y municipios) usando `unidecode` y funciones personalizadas.  
3. **Detección automática de indicadores** y aplicación de filtros opcionales (por año y producto).  
4. **Agregación departamental** mediante operaciones de suma (`sum`) o promedio (`mean`).  
5. **Unión con el shapefile** y estandarización del CRS (EPSG:4686, MAGNA-SIRGAS).  
6. **Generación de mapas temáticos** con `matplotlib`.  









