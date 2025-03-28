# 🧠 Portafolio de Proyectos ETL con PySpark + AWS

Este repositorio contiene 5 proyectos tipo ETL desarrollados en PySpark, integrando servicios de Amazon Web Services (AWS) como Amazon S3, Redshift y más. Todos los proyectos están diseñados para ejecutarse en notebooks de Jupyter y pueden ser orquestados fácilmente con Apache Airflow.

---

## 📁 Estructura del repositorio

```bash
ETL-PYSPARK-AWS/
│
├── notebooks/
│   ├── ETL_logs_web.ipynb
│   ├── ETL_datos_meteorologicos.ipynb
│   ├── ETL_tweets_sentimiento.ipynb
│   ├── ETL_ventas_retail.ipynb
│   └── ETL_facturacion_electronica.ipynb
│
├── airflow/
│   └── dag_ejemplo.py
│
├── data/
│   └── ejemplo.csv  # (Opcional: muestra o link a dataset)
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📅 Lista de proyectos

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
- Amazon Redshift / Aurora / DynamoDB
- AWS Glue Catalog
- Apache Airflow (para orquestación)

---

## 🚀 Instrucciones para ejecutar

1. Clonar este repositorio:
```bash
git clone https://github.com/Data-Engineer-FJ/ETL-PYSPARK-AWS.git
```

2. Instalar las dependencias:
```bash
pip install -r requirements.txt
```

3. Configurar tus credenciales de AWS (ej. `~/.aws/credentials` o variables de entorno).

4. Abrir los notebooks con Jupyter:
```bash
jupyter notebook
```

5. Ejecutar cada notebook paso a paso.

---

## 🔄 Orquestación con Airflow (opcional)

Para ejecutar estos pipelines con Airflow:
1. Ir al directorio `airflow/`.
2. Configurar el DAG `dag_ejemplo.py` con el operador `PapermillOperator` o `SparkSubmitOperator`.
3. Iniciar el entorno Airflow y activar el DAG.

---

## 📊 Ejemplo de resultado

Incluye capturas de pantalla o enlaces a visualizaciones generadas con los datos procesados (QuickSight, Tableau, etc.)

---

## ✍️ Contribuciones

Las contribuciones son bienvenidas. Por favor abre un issue o un pull request si deseas mejorar este repositorio.

---

## ✉️ Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.

---

## 🌟 Autor

Desarrollado por [Fredy Johel](https://github.com/Data-Engineer-FJ) | Data Engineer especializado en pipelines de datos, AWS y soluciones escalables.

