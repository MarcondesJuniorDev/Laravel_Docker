# Laravel 10.x

## Passo a passo para rodar o projeto
Clone o projeto
```sh
git clone https://github.com/MarcondesJuniorDev/Laravel laravel10
```
```sh
cd laravel10/
```


Crie o Arquivo .env
```sh
cp .env.example .env
```


Atualize essas variáveis de ambiente no arquivo .env
```dosini
APP_NAME="Laravel 10"
APP_URL=http://localhost:9001

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=[nome_que_desejar_db]
DB_USERNAME=[nome_usuario]
DB_PASSWORD=[senha_aqui]

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
```


Suba os containers do projeto
```sh
docker-compose up -d
```


Acesse o container
```sh
docker-compose exec app bash
```


Instale as dependências do projeto
```sh
composer install
```


Gere a key do projeto Laravel
```sh
php artisan key:generate
```


Acesse o projeto
[http://localhost:9001](http://localhost:9001)
