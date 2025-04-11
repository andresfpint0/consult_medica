# Sistema de Gestión de Pacientes

Este proyecto es un sistema completo de registro y consulta de pacientes. Incluye
- Backend en Laravel con arquitectura MVC
- API RESTful en PHP puro con autenticación JWT
- Frontend HTML/CSS/JS que consume la API
- Base de datos MySQL con migraciones y seeders

# Estructura de proyecto
/api-rest-php            # API RESTful en PHP
/api-rest-php/frontend   # Frontend HTML + Bootstrap
/consult_medica          # Backend en Laravel


# Tecnologías usadas

- PHP 8+
- Laravel 10+
- MySQL
- Bootstrap 
- JavaScript (fetch API)
- JWT para autenticació
- PDO para conexión segura en PHP puro


# Instalación y ejecución
1. Clonar el repositorio: 
https://github.com/andresfpint0/consult_medica.git

2. Configurar la base de datos
Crea una base de datos en MySQL y ajusta tus archivos .env en Laravel y configuración en PHP
create database consult_medica;

3. Laravel backend
cd laravel-backend
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve

4. API RESTful en PHP
cd api-rest-php

5. Frontend
/frontend/index.html

# Autenticación
- El sistema usa JWT.
- Al iniciar sesión (por ejemplo, desde /login.html), se genera un token guardado en localStorage.
- Este token se incluye en cada solicitud a la API usando el header Authorization: Bearer <token>.

# Pruebas
- Laravel incluye pruebas con PHPUnit (php artisan test)
- API PHP tiene pruebas con PHPUnit también

