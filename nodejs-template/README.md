# Plantilla Node.js con Podman Compose

## Instrucciones

1. Clona este repositorio.
2. Navega al directorio `nodejs-template`.
3. Ejecuta `podman-compose up -d` para iniciar el servidor.

### Archivos Clave
- `compose.yml`: especifica el contenedor para Node.js (API) + Postgres + Redis.


## Archivos Sugeridos
- ops/node.Dockerfile: multi-stage (builder + runtime), expone PORT, instala deps, no como root.