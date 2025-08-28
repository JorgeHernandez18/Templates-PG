# Plantilla React con Podman Compose

## Instrucciones

1. Clona este repositorio.
2. Navega al directorio `react-template`.
3. Ejecuta `podman-compose up -d` para correr la aplicación frontend.

### Contenido
- `compose.yml`: define el servicio de ReactJS (build de producción) + Nginx

## Archivos Sugeridos
- ops/react-nginx.Dockerfile / usar nginx.conf con SPA fallback.

- Para AngularJS 1.x (proyecto legacy), el ./dist proviene de tu herramienta de build (gulp/grunt/webpack).