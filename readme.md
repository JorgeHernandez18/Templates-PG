# Templates de Podman Compose para Proyectos Web

Este repositorio contiene **ejemplos listos de `compose.yaml`** para levantar entornos de desarrollo con **Podman** (compatibles con Docker Compose).  
Incluye configuraciones reales y comunes vistas en proyectos productivos.

Stacks disponibles:

- 🟢 AngularJS (servido con Nginx)  
- 🔵 Laravel (Nginx + PHP-FPM + MySQL + Redis + Workers)  
- 🟣 Node.js (API + PostgreSQL + Redis)  
- 🟡 ReactJS (build de producción servido con Nginx)  
- 🟠 Spring Boot (Java + PostgreSQL)  

---

## 📦 Tecnologías y Descripción de los Templates

### 1. AngularJS
Un entorno para servir aplicaciones AngularJS estáticas con **Nginx** como servidor web.  
Incluye configuración de volúmenes para mapear los archivos compilados (`dist/`) y exponerlos en el puerto `8080`.

---

### 2. Laravel
Un stack clásico de **Laravel + PHP-FPM + Nginx + MySQL**.  
La base de datos se configura con variables de entorno, y los volúmenes permiten el desarrollo sin perder datos de la DB.

---

### 3. NodeJS
Una aplicación backend en Node.js con soporte para hot-reload en desarrollo (gracias a `nodemon`) y configuración de puerto a través de `.env`.  

---

### 4. ReactJS
Un entorno React con **Nginx** para servir la build de producción (`npm run build`).  
Se expone en el puerto `3000` y permite mapear el directorio `build/`.

---

### 5. Spring Boot
Un contenedor con una aplicación **Spring Boot + PostgreSQL**.  
Se construye desde un `Dockerfile` que empaqueta el `.jar` y se conecta a la base de datos PostgreSQL configurada con variables en `.env`.

---

# 🚀 Cómo ejecutar

## 1. Clonar el repositorio
git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo

## 2. Entrar a la carpeta del proyecto (ejemplo con Laravel)
cd laravel

## 3. Crear el archivo .env
cp .env.example .env

## 4. Levantar el servicio con Podman Compose
podman-compose up -d
