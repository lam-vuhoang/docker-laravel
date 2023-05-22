# Setup
After pull the source code, run this command on terminal 
```shell
docker compose up -d
```
## Install laravel
### Give permission
```shell
sudo chmod -R 777 backend
```
### Create laravel project
```shell
docker compose run --rm composer create-project laravel/laravel backend
```
### Move project to backend folder
```shell
sudo cp -a  backend/backend/. backend/
```
```shell
sudo rm -r backend/backend
```
### Install composer
```shell
docker compose run --rm composer install
```
### Check if it works
```shell
docker compose run --rm artisan serve
```

# Interaction
## To run composer
```shell
docker compose run composer --version
```

## To run npm 
```shell
docker compose run npm --version
```
## To run artisan
```shell
docker compose run artisan --version
```