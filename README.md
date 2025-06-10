# Laravel Store

## Requirement
- Laravel 12.x
- PHP 8.3
- MySQL 8.0
- Docker
- Docker Compose

## Local Development
- Clone Repository
- Run `cp .env.example .env`
- Run `php artisan key:generate`
- Run `docker compose up -d --build`
- Buka browser, ketikkan `localhost:8012`.

## Migration
Migration dijalankan terpisah diluar eksekusi inisiasi.
### Langkah Migration
```bash
docker exec -it laravel12_app bash
php artisan migrate
exit
```
