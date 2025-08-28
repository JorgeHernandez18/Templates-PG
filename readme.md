# 📦 Plantillas Podman Compose para Proyectos de Grado

Este repositorio contiene plantillas `podman-compose.yml` para facilitar el despliegue de aplicaciones comúnmente usadas en proyectos de grado en la universidad. Las plantillas están listas para usarse y adaptarse a las necesidades de cada proyecto.

---

## 🧰 Requisitos Generales

- Tener instalado Podman y Podman Compose. (Compatible con Docker)
- Copiar la plantilla correspondiente al lenguaje/framework de tu proyecto.
- Asegurarte de que tu código esté en el mismo nivel del `podman-compose.yml` o configurar correctamente los volúmenes.

---
## Ejemplo de .env
# Base DB
POSTGRES_DB=app
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres

# MySQL (Laravel)
DB_DATABASE=laravel
DB_USERNAME=laravel
DB_PASSWORD=secret
DB_ROOT_PASSWORD=root

# Node/React
NODE_ENV=production
PORT=3000

# Spring
SERVER_PORT=8080
SPRING_PROFILES_ACTIVE=prod


