# Estadística Aplicada a Datos con Python - Tutorial de Data Science

Bienvenido a este repositorio, donde comparto un tutorial práctico sobre **estadística aplicada a datos** utilizando **Python**. Este proyecto surge de mi experiencia trabajando en análisis de transacciones y ventas de un restaurante local, y está diseñado para ayudar a quienes desean aprender a transformar datos en insights valiosos para la toma de decisiones.

Este repositorio acompaña mi blog en Medium donde explico detalladamente cada paso del análisis, desde la preparación de datos hasta la interpretación de resultados. ¡Te invito a leer el artículo completo para profundizar en cada concepto!

## Descripción del Proyecto

En este tutorial, aplico conceptos fundamentales de estadística (media, mediana, varianza, desviación estándar) para analizar un dataset real. Se abordan pasos como:
- **Carga y Preparación de Datos:** Conversión de formatos, limpieza y verificación de integridad.
- **Estadísticas Descriptivas:** Cálculo de medidas de tendencia central y dispersión.
- **Visualización de Datos:** Uso de histogramas, boxplots y gráficos de barras para interpretar la distribución y variabilidad.
- **Análisis por Categoría e Ingresos:** Comparación de ventas por producto, tipo de artículo y franjas horarias.

Este repositorio incluye notebooks y scripts que puedes ejecutar para replicar el análisis, así como visualizaciones que muestran las conclusiones alcanzadas.

## Contenido del Repositorio

- **README.md:** Esta documentación.
- **ventas_cafeteria.csv:** el dataset (transacciones de un restaurante local).
- **Analisis_con_estadistica.ipynb**: Google colab con el análisis detallado.

## Descripción del csv

El DataFrame que estamos analizando proviene de un restaurante local y cuenta con 1000 registros distribuidos en 10 columnas. Cada fila representa una transacción de venta, y las columnas se describen de la siguiente manera:

- id_pedido: Identificador único de cada transacción.
- fecha: La fecha en que se realizó la transacción (originalmente en formato texto, que se recomienda convertir a datetime para análisis temporal).
- nombre_articulo: Nombre del artículo vendido, donde destacan ítems como Café frío, Jugo natural, Empanada, entre otros.
- tipo_articulo: Categoría del artículo, principalmente clasificados en dos grupos: Comida rápida y Bebidas. Se observa que la mayoría (686 registros) corresponde a comida rápida, mientras que 314 son bebidas.
- precio_articulo: Precio unitario del artículo, con valores que varían entre 20 y 60, donde el precio más común es 20.
- cantidad: Número de unidades vendidas en cada transacción, con una media de alrededor de 8 artículos por pedido.
- monto_transaccion: Valor total de la transacción, calculado como el producto de precio_articulo y cantidad. Los montos varían considerablemente, con una media de 275.23 y mediana de 240, lo que sugiere cierta asimetría en la distribución.
- tipo_transaccion: Forma de pago utilizada, ya sea Efectivo (476 transacciones) o En línea (417 transacciones), aunque esta columna presenta algunos valores nulos.
- recibido_por: Género de la persona que atendió la transacción, casi equilibrado entre Hombre (512) y Mujer (488).
- hora_venta: Franja horaria en la que se realizó la venta, categorizada en Mañana, Tarde, Atardecer, Noche y Medianoche, mostrando una distribución relativamente uniforme con ligeras variaciones.
