# Proyecto N · [Título del proyecto]

## Descripción y objetivo

El problema a desarrollar en este es predecir mediante ciertos datos, las condiciones optimas para la produccion de cultivos ( por ejemplo: tubérculos), los datos que se recopilan son la temperatura, la humedad , la concentracion de CO2 y la calidad de agua.
Al final se obtiene la visualizacion de los datos en tiempo real permitiendo monitorización y análisis interactivo en un dashboard.

## Arquitectura

```mermaid
graph LR
    A[Sensores ] --> B[Ingesta con Kafka]
    B --> C[Fiware + CreateDB] 
    C --> D[Consultas / indicadores]
    D --> E[Grafana / Power BI]