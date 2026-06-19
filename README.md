# DevOps Interview — Prueba Técnica

> **Importante:** la prueba técnica completa debe ser entregada en un único repositorio.

Este repositorio contiene las tres pruebas técnicas a resolver. Cada una tiene su propio directorio con la consigna detallada.

```
.
├── prueba-1/   # Diagrama de red
├── prueba-2/   # Deployment Django + React.js
└── prueba-3/   # CI/CD con nginx
```

## Desafíos opcionales

Cada prueba incluye una sección de **desafío adicional** con una actividad de mayor complejidad.

| Nivel | Desafíos adicionales |
|-------|----------------------|
| **Trainee / Junior** | Son opcionales. Si te animás a intentarlos, aunque sea parcialmente, es una buena forma de mostrar curiosidad e iniciativa. No resolverlos no penaliza la evaluación. |
| **Semi Senior** | Son **requisito**. Se espera que estén resueltos y justificados junto con las pruebas base. |

---

## Prueba 1 — Diagrama de red

Diseñar la arquitectura de una aplicación web en AWS o GCP y producir un diagrama de red acompañado de una descripción escrita. La arquitectura debe soportar cargas variables, alta disponibilidad, frontend en JS, base de datos relacional y no relacional, y consumo de 2 microservicios externos.

**Desafío adicional:** estimación de costos de la arquitectura con análisis de trade-offs.

→ [Consigna completa](prueba-1/README.md)

## Prueba 2 — Deployment Django + React.js

Dockerizar la aplicación incluida en este repositorio (backend Django + frontend React.js) y desplegarla con un único `docker-compose`. Se deben entregar los Dockerfiles, el archivo de compose e instrucciones para correr la aplicación tanto en local como en la nube.

**Desafío adicional:** desplegar la aplicación en un cluster de Kubernetes local (kind o minikube) con los manifests correspondientes.

→ [Consigna completa](prueba-2/README.md)

## Prueba 3 — CI/CD con nginx

Dockerizar un nginx con un `index.html` customizado e implementar un pipeline de CI/CD que, ante cada cambio en ese archivo, buildee la nueva imagen y actualice el servicio automáticamente en la plataforma elegida.

**Desafío adicional:** diseñar un flujo de trabajo completo tratando al nginx como el frontend estático de una app real (estrategia de branching, versionado de imágenes y rollback).

→ [Consigna completa](prueba-3/README.md)
