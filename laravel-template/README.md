# Plantilla Laravel con Podman Compose

## Instrucciones

1. Clona este repositorio.
2. Navega al directorio `laravel-template`.
3. Ejecuta `podman-compose up -d` para iniciar el proyecto.

### Estructura de Archivos
- `compose.yml`: Contiene los servicios de Laravel + Nginx + PHP-FPM + MySQL + Redis + Queue/Scheduler.

## Archivos Sugeridos
- ops/php-fpm.Dockerfile: PHP 8.2 con extensiones (pdo_mysql, redis, gd, intl, opcache).

- ops/nginx.conf: server para /public.

- .env con DB_*, REDIS_*, APP_KEY, etc. Puedes basarte en Laravel Sail para ideas de servicios
