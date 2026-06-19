# Prueba 1 — Diagrama de Red

## Consigna

Producir un diagrama de red de una aplicación web en **GCP o AWS** y escribir una descripción de texto de entre media y una página explicando las elecciones realizadas y la arquitectura propuesta.

Se puede utilizar cualquier herramienta de diagramación (LucidChart, draw.io, Excalidraw, etc.).

## Requisitos del diseño

La arquitectura debe soportar:

- Cargas variables
- Alta disponibilidad (HA)
- Frontend en JavaScript
- Backend con una base de datos relacional y una no relacional
- El backend consume 2 microservicios externos

El diagrama debe hacer uso de soluciones distribuidas.

## Entregables

- Diagrama de red (imagen o link al diagrama)
- Descripción escrita (entre media y una página) explicando:
  - Las decisiones de arquitectura tomadas
  - Por qué se eligieron los servicios utilizados
  - Cómo se satisface cada uno de los requisitos listados arriba

---

## Desafío adicional _(opcional)_

> Esta sección no es un requisito. Si querés ir un paso más allá, es una buena oportunidad para mostrar criterio técnico sobre costos.

Usando la [calculadora de precios de AWS](https://calculator.aws/pricing/2/home) o la [de GCP](https://cloud.google.com/products/calculator), estimá el costo mensual de la arquitectura propuesta.

Se espera:

- Un desglose por servicio con los valores estimados
- Una breve justificación de los parámetros elegidos (región, tamaño de instancias, tráfico estimado, etc.)
- Al menos un trade-off analizado: ¿qué cambiarías si el presupuesto fuera un 30% menor? ¿y si el tráfico se duplicara?

El objetivo no es dar un número exacto sino demostrar que se puede razonar sobre costo y arquitectura al mismo tiempo.
