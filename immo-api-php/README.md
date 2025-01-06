# Slim 4 API

Simple API using Slim v4 MySQL and optionnaly S3 Storage

## Run

- Create `.env` from `.env.exemple`
- Update environement variable
- run `php -S localhost:<PORT> -t ./public`

## Start docker

docker compose -d

docker exec -it php_web bash

### Etapes

#### Mettre à jour les paquets
apt-get update

#### Installer zip, unzip, et git
apt-get install -y zip unzip git

#### Activer l'extension zip pour PHP
docker-php-ext-install zip

#### Télécharger le script d'installation de Composer
curl -sS https://getcomposer.org/installer | php

#### Déplacer le binaire Composer pour le rendre globalement accessible
mv composer.phar /usr/local/bin/composer

#### Vérifier que Composer est installé
composer install

