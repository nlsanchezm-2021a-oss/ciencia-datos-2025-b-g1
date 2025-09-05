# 📄 Documento Comparativo – Arquitecturas Big Data

## 1. Escenario
El caso de análisis será **HealthData Solutions**, una empresa del sector salud que procesa:  
- Registros clínicos electrónicos de miles de pacientes en hospitales y clínicas.  
- Resultados de exámenes de laboratorio y dispositivos médicos.  
- Datos IoT de sensores para monitoreo en tiempo real de pacientes (pulso, glucosa, presión arterial, etc.).  

El reto es manejar grandes volúmenes de información médica garantizando **seguridad, escalabilidad y analítica avanzada**, de modo que se optimicen diagnósticos, se mejore la gestión hospitalaria y se eleve la calidad de atención al paciente.


## 2. Introducción

### Propósito
Comparar tres arquitecturas Big Data (Hadoop, Spark y Nube) evaluando sus componentes, ventajas, limitaciones y aplicaciones en el sector salud, con el fin de determinar la más adecuada para HealthData Solutions.

### Alcance
El análisis se centrará en:  
- **Hadoop:** modelo clásico basado en HDFS, YARN y MapReduce.  
- **Apache Spark:** plataforma de procesamiento en memoria con soporte batch y streaming.  
- **Arquitecturas en la nube (ej. AWS, GCP, Azure):** servicios gestionados con escalabilidad y seguridad integrada.  

### Glosario
- **HDFS:** sistema distribuido para almacenar grandes volúmenes de datos clínicos.  
- **YARN:** gestor de recursos en Hadoop.  
- **MapReduce:** modelo de programación batch.  
- **RDD:** dataset distribuido tolerante a fallos en Spark.  
- **ETL:** proceso de extracción, transformación y carga de datos.  
- **Escalabilidad automática:** capacidad de la nube para ajustar recursos sin intervención manual.  


## 3. Descripción de arquitecturas

### a) Hadoop
- **Componentes:** HDFS, YARN, MapReduce, Hive, HBase.  
- **Ventaja:** almacenamiento económico y confiable de historiales médicos y estudios previos.  
- **Limitación:** latencia alta, no apto para monitoreo en tiempo real de pacientes.  

### b) Apache Spark
- **Componentes:** Spark Core, RDD, Spark SQL, MLlib, Streaming.  
- **Ventaja:** análisis en tiempo real de signos vitales y resultados clínicos.  
- **Limitación:** requiere clústeres potentes con mayor memoria.  

### c) Arquitecturas en la nube
- **Componentes:** servicios gestionados (AWS EMR, BigQuery, Azure Synapse), auto-escalado, data lakes.  
- **Ventaja:** escalabilidad inmediata, integración con IoT y seguridad avanzada.  
- **Limitación:** dependencia del proveedor y costos variables.