---
layout: post
title: "Análisis de Clickstream con Spark"
date: 2025-10-29
categories: analytics spark
---

# Análisis de Flujo de Datos con Spark

Este es mi análisis de clickstream usando Apache Spark.

## Objetivo

Procesar datos de navegación en tiempo real para detectar patrones.

## Resultados

Se procesaron 1000 registros de 50 usuarios únicos.

### Código Python
```python
from pyspark.sql import SparkSession

spark = SparkSession.builder \
    .appName("ClickstreamAnalysis") \
    .getOrCreate()
```

## Conclusiones

El streaming es esencial para competitividad en 2025.