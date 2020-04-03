### Laravel Docker Starter Kit

#### Services

* [NGINX](https://hub.docker.com/_/nginx) (alpine)
* [MySQL 5.7](https://hub.docker.com/_/mysql)
* [PHP 7.4.3](https://hub.docker.com/_/php)
* [Composer](https://hub.docker.com/_/composer)
* [Laravel 7.*](https://laravel.com/docs/7.x)
* PHP Packages
    * [barryvdh/laravel-debugbar](https://packagist.org/packages/barryvdh/laravel-debugbar)
    * [barryvdh/laravel-ide-helper](https://packagist.org/packages/barryvdh/laravel-ide-helper)
    * [nunomaduro/larastan](https://packagist.org/packages/nunomaduro/larastan)

#### Configuration

1. Create `.env` file:

    ```bash
    cp .env.example .env
    ```

2. Add `APP_USER` variable:

    ```ini
    APP_USER=serge
    ```
   
3. Fill `DB_*` credentials:

    ```ini
    DB_CONNECTION=mysql
    DB_HOST=app-storage
    DB_PORT=3306
    DB_DATABASE=laravel
    DB_USERNAME=laravel
    DB_PASSWORD=secret
    ```
   
4. Build Docker environment:

    ```bash
    docker-compose build
    ```

5. Run Docker environment:

    ```bash
    docker-compose up
    ```
6. Install `Composer` vendors:

    ```bash
    docker-compose exec app-php composer install
    ```

7. Add site domain to `/etc/hosts` file (Linux):

    ```text
    127.0.0.1 local-app.test
    ```
