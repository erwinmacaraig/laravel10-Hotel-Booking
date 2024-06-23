#Laravel Setup for Docker

### Build the container
```
docker compose up -d --build
```

### To run command in a container
```
docker compose run --rm php-laravel /bin/sh
```

### Create Laravel project
Create or go to source code directory within the project and execute

```
docker compose run --rm composer create-project laravel/laravel .
```

### If access forbidden
```
docker compose run --rm php-laravel /bin/sh
```
and then
```
chown -R laravel:laravel /var/www/html


