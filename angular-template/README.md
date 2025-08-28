# Plantilla Angular con Podman Compose

## Instrucciones

1. Clona este repositorio.
2. Navega al directorio `angular-template`.
3. Ejecuta `podman-compose up -d` para lanzar el proyecto Angular.

### Archivos
- `compose.yml`: configura el entorno AngularJS (estático) + Nginx.

### Archivos Sugeridos
- ops/react-nginx.Dockerfile / usar nginx.conf con SPA fallback.

- Para AngularJS 1.x (proyecto legacy), el ./dist proviene de tu herramienta de build (gulp/grunt/webpack).
