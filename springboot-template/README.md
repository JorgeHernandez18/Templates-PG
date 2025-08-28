# Plantilla Spring Boot con Podman Compose

## Instrucciones

1. Clona este repositorio.
2. Navega al directorio `springboot-template`.
3. Ejecuta `podman-compose up -d` para iniciar el proyecto.

### Estructura de Archivos
- `compose.yml`: define los servicios para Spring Boot + PostgreSQL (con perfiles).

## Archivos Sugeridos
- ops/spring.Dockerfile: multi-stage con Maven/Gradle y JRE Temurin 21.
