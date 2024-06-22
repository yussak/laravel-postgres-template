## Laravelのトップページを表示
1. git clone $ git clone https://github.com/yussak/laravel-postgres-template.git {ディレクトリ名}
2. cd ディレクトリ名
3. docker-compose up -d
4. docker-compose exec app bash
5. composer install
6. cp .env.example .env
7. php artisan key:generate
8. locahost:8000にアクセスするとLaravelのトップページが表示される

## migration
1. .envを以下のように変える
```
DB_CONNECTION=pgsql
DB_HOST=db
DB_PORT=5432
DB_DATABASE=laravel
DB_USERNAME=laravel
DB_PASSWORD=secret
```
2.  docker-compose exec app bash
3.  php artisan migrate
