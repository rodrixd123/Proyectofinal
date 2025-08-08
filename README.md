# **Proyecto ETL: Migración de Datos de SQL Server a BigQuery usando Google Colab**  

## **Descripción**  
Este proyecto implementa un proceso **ETL (Extract, Transform, Load)** para migrar datos desde un entorno **OLTP (SQL Server)** hacia un entorno **OLAP (Google BigQuery)**.  
La extracción se realiza a partir de archivos **CSV** generados desde la base de datos SQL Server, los cuales se procesan en **Google Colab** y posteriormente se cargan al dataset `VentasDW` en BigQuery.  

---

## **Objetivos**  
- Extraer datos desde SQL Server y almacenarlos en CSV.  
- Realizar limpieza y transformación de datos en Python usando Pandas.  
- Cargar la información final en Google BigQuery.  

---

## **Tecnologías Utilizadas**  
- **Python** (Google Colab)  
- **Pandas**  
- **Google Cloud BigQuery**  
- **Google Drive** (almacenamiento intermedio de CSV)  
- **GitHub** (documentación y control de versiones)  

---

## **Flujo del Proceso**  
1. **Extracción:**  
   - Se exportaron las tablas de SQL Server en formato CSV.  
   - Los archivos CSV se comprimieron en un ZIP (`DataBig2025.zip`).  

2. **Transformación:**  
   - Lectura de los CSV desde Google Drive.  
   - Conversión de codificaciones y limpieza de datos para evitar errores de lectura (`UTF-8` / `latin-1`).  

3. **Carga:**  
   - Subida de cada CSV como una tabla independiente en el dataset `VentasDW` de Google BigQuery.  

---

## **Ejecución del Proyecto**  
1. Abrir el notebook en Google Colab.  
2. Montar Google Drive para acceder a los archivos CSV.  
3. Configurar credenciales de Google Cloud.  
4. Ejecutar el código de carga a BigQuery.  

---



