# Prueba 2 — Deployment Django + React.js

## Consigna

Elaborar el deployment dockerizado de la aplicación contenida en este directorio: backend en **Django** y frontend en **React.js**. Todos los servicios deben desplegarse con un único `docker-compose`.

## Requisitos

- Crear los **Dockerfiles** necesarios para el backend y el frontend
- Definir un `docker-compose.yml` que levante todos los servicios juntos
- Justificar la forma en que se elaboró el deployment (uso de supervisor, scripts, docker-compose, kubernetes, etc.)

## Entregables

- `Dockerfile` del backend
- `Dockerfile` del frontend
- `docker-compose.yml` en la raíz de esta carpeta
- Este `README.md` actualizado con:
  - Instrucciones detalladas para compilar y levantar la aplicación en local
  - Instrucciones para desplegarla en la nube (AWS o GCP)
  - Justificación de las decisiones tomadas

## Estructura del proyecto

```
prueba-2/
├── backend/    # Aplicación Django
└── frontend/   # Aplicación React.js
```

---

## Desafío adicional _(opcional)_

> Esta sección no es un requisito. Si querés profundizar, es una buena oportunidad para mostrar conocimiento de orquestación de contenedores.

En lugar de (o además de) docker-compose, desplegá la aplicación en un **cluster de Kubernetes local** usando [kind](https://kind.sigs.k8s.io/) o [minikube](https://minikube.sigs.k8s.io/).

Se espera:

- Manifests de Kubernetes para cada servicio: `Deployment`, `Service` e `Ingress`
- El cluster debe poder levantarse siguiendo las instrucciones del README sin pasos manuales adicionales
- Explicar brevemente por qué elegiste esa estructura de manifests y cómo manejarías las variables de entorno y secretos en un ambiente real

No es necesario usar Helm ni implementar autoscaling; alcanza con que la aplicación funcione y esté correctamente organizada.
