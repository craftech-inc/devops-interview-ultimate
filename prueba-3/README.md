# Prueba 3 — CI/CD con nginx

## Consigna

Dockerizar un nginx con el `index.html` por defecto. Elaborar un pipeline que, ante cada cambio en el `index.html`, buildee la nueva imagen y la actualice en la plataforma elegida.

## Requisitos

- Crear un `Dockerfile` para el nginx con su `index.html`
- Implementar un pipeline de CI/CD que:
  - Se dispare automáticamente ante cambios en el `index.html`
  - Buildee la nueva imagen Docker
  - Actualice el servicio en la plataforma elegida

**Plataformas de deploy sugeridas:** docker-compose, Docker Swarm, Kubernetes

**Herramientas de CI/CD sugeridas:** CircleCI, GitLab CI, GitHub Actions, Bitbucket Pipelines

## Entregables

- `Dockerfile` del nginx
- Archivo de configuración del pipeline (`.github/workflows/`, `.gitlab-ci.yml`, etc.)
- Este `README.md` actualizado con:
  - Explicación del pipeline implementado
  - Instrucciones para replicar el entorno
  - Justificación de las herramientas y plataforma elegidas

---

## Desafío adicional _(opcional)_

> Esta sección no es un requisito. Si querés ir más allá, es una oportunidad para diseñar un flujo de trabajo completo como el que se usaría en un proyecto real.

Pensá en el nginx como si fuera el frontend estático de una aplicación real y diseñá el flujo de trabajo completo a su alrededor. Algunos puntos a resolver:

**Estrategia de branching y ambientes**
- ¿Cómo diferenciarías un deploy a desarrollo de uno a producción?
- ¿Qué ramas disparan qué ambientes?

**Versionado de imágenes**
- ¿Cómo taggeás las imágenes para poder identificar qué versión está corriendo en cada ambiente?
- ¿Cómo evitás usar siempre `latest`?

**Rollback**
- Si el deploy de una nueva versión falla o genera un error, ¿cómo volvés a la versión anterior?

No hay una única respuesta correcta. Lo que se evalúa es la capacidad de razonar sobre un flujo de trabajo real, identificar problemas potenciales y proponer soluciones concretas. Podés resolverlo con código, con un diagrama, o con una descripción escrita.
