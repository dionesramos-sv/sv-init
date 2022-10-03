# Initial Installation
Developed in Wordpress using roots/sage

## Environment settings
In the root of the project there is a file called `.env`, which has all the important information in global variables of the `wp-config.php` file.

## Installing global dependencies
Follow the instructions before starting to develop on the project:

- Install [Docker Compose](https://docs.docker.com/compose/install) following the instructions in https://docs.docker.com/compose/install

## Configuring the project
Configure the project by following the steps:

1. Set the `PROJECT_NAME` variable on `.env` file

2. Set the `THEME_NAME` variable on `.env` file

3. Set `SECRET KEYS` variables on `.env` file, getting from [secret keys](https://api.wordpress.org/secret-key/1.1/salt/)

4. Run the following command:

        docker-compose up -d

5. In case you need to update your ```composer``` dependencies, delete the ```composer.lock``` and run ```docker-compose run <config | themebackend>```

## Access
- Site: http://localhost/
- Dashboard: http://localhost/wp-admin/
- Site with hot reload: http://localhost:3000/
- phpMyAdmin: http://localhost:8080/
- - Login: root
- - Password: root
- MailHog: http://localhost:8025
