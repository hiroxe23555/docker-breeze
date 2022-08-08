#Laravel8+Breeze認証+Ineatia+react+docker
##PHP8・Laravel8・react・mysql・Nginx・docker・phpdebug3
##docker-compose起動
```sh
cd docker-breeze
docker-compose build
docker-compose up -d
```
#コンテナごとの処理
##app-dlコンテナに入る
```sh
docker-compose exec app-dl bash
composer create-project laravel/laravel:^8.0  my-app
composer require laravel/breeze:^2.1 --dev
php artisan breeze:install react
npm install && npm run dev
```
##db-dlコンテナに入る
```sh
docker-compose exec db-dl bash
mysql -u root -p
create database test_db;
```







