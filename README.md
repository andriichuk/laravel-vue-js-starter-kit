## Laravel VueJS Starter Kit

Features

* [Laravel 8.x](https://laravel.com/docs/8.x/installation)
    * [Sail (PHP 7.4)](https://laravel.com/docs/8.x/sail)
* [VueJS 2.x](https://vuejs.org/v2/guide/)
    * [Vuex](https://vuex.vuejs.org/)
    * [Vue Router](https://router.vuejs.org/)

### Installation

Clone this repository

```shell
git clone git@github.com:andriichuk/laravel-vue-js-starter-kit.git
```

Up Docker containers for the first time

```shell
composer install

./vendor/bin/sail up
```

Install composer dependencies in the next time

```shell
./vendor/bin/sail composer install
```

Fill in environment variables

```shell
cp .env.example .env
```

Install and run `npm` watch task

```shell
./vendor/bin/sail npm install && npm run watch
```

Update `hosts` file

```text
127.0.0.1 laravel.test
```

Open [laravel.test](http:://laravel.test) in the browser
