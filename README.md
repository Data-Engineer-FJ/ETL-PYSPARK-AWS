
# 🧠 Portafolio de Proyectos ETL con PySpark + AWS

Este repositorio contiene 5 proyectos tipo ETL desarrollados en PySpark, integrando servicios de Amazon Web Services (AWS) como Amazon S3, Redshift y más. Todos los proyectos están diseñados para ejecutarse en notebooks de Jupyter y pueden ser orquestados fácilmente con Apache Airflow.

---

## 📁 Lista de proyectos

1. **ETL de Logs Web**
   - Fuente: Logs en texto plano en Amazon S3
   - Transformación: Extracción de códigos 404, limpieza de logs
   - Destino: Amazon S3 (Parquet)

2. **ETL de Datos Meteorológicos**
   - Fuente: CSVs meteorológicos en S3
   - Transformación: Cálculo de temperatura media y limpieza
   - Destino: Amazon S3 (Parquet)

3. **ETL de Tweets para Análisis de Sentimiento**
   - Fuente: JSONs desde la API de Twitter
   - Transformación: Limpieza de texto, análisis de sentimiento
   - Destino: Redshift o DynamoDB

4. **ETL de Ventas Retail**
   - Fuente: Datos CSV de puntos de venta (POS)
   - Transformación: Cálculo de total por venta
   - Destino: Amazon S3 o Redshift

5. **ETL de Facturación Electrónica**
   - Fuente: Archivos JSON/XML de comprobantes electrónicos
   - Transformación: Extracción de RUC, monto y fecha
   - Destino: Aurora PostgreSQL o Amazon S3

---

## ⚙️ Tecnologías usadas

- Apache Spark (PySpark)
- Jupyter Notebook
- Amazon S3
- Amazon Redshift / Aurora
- AWS Glue Catalog
- Apache Airflow (opcional para orquestación)

---

## 🚀 Cómo correr los notebooks

1. Configura tus credenciales de AWS.
2. Instala las dependencias necesarias (PySpark, boto3).
3. Abre el notebook correspondiente en Jupyter.
4. Ejecuta las celdas paso a paso.

---

## 📌 Orquestación con Airflow (opcional)

Puedes automatizar estos flujos con **Apache Airflow** creando DAGs personalizados que ejecuten notebooks usando operadores como `PapermillOperator` o scripts PySpark directamente en EMR o ECS.

---

## ✨ Autor

Proyecto desarrollado por un Data Engineer apasionado por la nube, los datos y las soluciones escalables.

---
