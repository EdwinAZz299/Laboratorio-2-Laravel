
# Laboratorio #2 – Implementación del Login en Laravel
## Unidad I: Modelo Vista Controlador (MVC)
### Tema de la Tarea
Documentar el repositorio del laboratorio en Laravel, incluyendo los requisitos previos, los
códigos implementados y los resultados obtenidos en la ejecución del laboratorio.

Nombre: Edwin Zhong
Profesora: Irina Fong
Grupo: 1SF-132
Curso: Ingieneria Web

## Instrucciones de la Tarea
### 1. Prerrequisitos (ecosistema de desarrollo del lab)

- PHP versión 8.0 o superior.
- Composer última versión estable.
- Laravel Installer o crear proyecto con laravel new /composer create-project.
- Paquete de servidor web local. (Entorno de Desarrollo)(ej.
XAMPP, WampServer o Laragon).
- Servidor web: Apache o Nginx
- Base de datos MySQL/MariaDB funcionando.
- Editor de código (Visual Studio Code recomendado).
- NPN: si fue necesario. Dejarlo en blanco de lo Contrario.
- Sistema Operativo:
Incluir iconos por Tecnología


 2. Incluir una introducción, que explique brevemente la función de las principales
carpetas en torno a la arquitectura MVC (controladores, rutas, vistas y modelos).
Además, documentar que comandos utilizó para las migraciones. El objetivo del
laboratorio.

3. Debe incluir una imagen que muestre el resultado visible de lo que le resultó hacer el
laboratorio.

4. Base de Datos. Expliquen el entorno: base de datos, los aspectos de laravel, en torno
al .env, migraciones, comandos que utilizó para levantar las tablas que necesitaba para
el laboratorio. Genere un respaldo (backup) de la base de datos y mantenga una copia
en su repositorio.

5. Dificultades y Soluciones: Describir los principales problemas encontrados durante el laboratorio (ej.
errores de migración, configuración del .env, instalación de dependencias).
6. Ubicar puntos de Referencias que le ayudaron a realizar el laboratorio ejemplo

## Flujo de instalación y comandos utilizados

Crear el proyecto Laravel:

composer create-project laravel/laravel:^11.0 myapp cd myapp

Instalar paquete de autenticación Breeze:

composer require laravel/breeze --dev php artisan breeze:install blade

Instalar dependencias frontend:

npm install npm run dev

Configuración de entorno:

cp .env.example .env php artisan key:generate

Migraciones para crear las tablas:

php artisan migrate

Levantar servidor de desarrollo:

php artisan serve

## Resultados del laboratorio
Resultado visible del login, registro y dashboard:

(Register.png)
![Register](https://github.com/user-attachments/assets/b34ead4a-e83b-4da3-aa18-cc9582daa976)

(Login.png)
![LoginListo](https://github.com/user-attachments/assets/7bd907aa-dbe3-42f0-9326-bcce542fb488)

## Dificultades y Soluciones
Error: “Vite manifest not found at public/build/manifest.json” Causa: no se habían compilado los assets de Vite. Solución: ejecutar npm install && npm run dev o npm run build.

Error: “Could not open input file: artisan” Causa: estaba fuera de la carpeta del proyecto. Solución: entrar con cd ~/myapp antes de ejecutar comandos.

## Referencias
Laravel. (s. f.). Laravel - The PHP Framework for Web Artisans. Recuperado el 28 de septiembre de 2025, de https://laravel.com/docs

Laravel. (s. f.). Starter Kits: Breeze. Recuperado el 28 de septiembre de 2025, de https://laravel.com/docs/starter-kits#breeze

Composer. (s. f.). Dependency Manager for PHP. Recuperado el 28 de septiembre de 2025, de https://getcomposer.org

## Footer
Este laboratorio fue desarrollado como parte del curso Ingeniería Web de la Universidad Tecnológica de Panamá.
