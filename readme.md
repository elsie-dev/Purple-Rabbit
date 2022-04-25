# Purple Rabbit

This is the job test if you wish to be a DevOps developer at Twentyfour

## Contents

When you have completed this test you will have demonstrated skills/knowledge in

- docker
- mariadb
- wordpress
- php
- nginx
- apache
- adminer/phpmyadmin

## Requirements

You'll need to have docker and docker-compose installed, you have to use the nginx as reverse proxy to a apache/httpd web server that then proxies to php-fpm. The reason we are doing it this way is so that you demonstrate you understand basic web server knowledge. You are free to choose your own images for the database, phpmyadmin. For php you have to use wordpress:phpX.X-fpm, so wordpress:php7.4-fpm. Would be valid, you cannot use a wordpress image that contains apache.

NGINX -> APACHE/HTTPD -> PHP-FPM

## Bonus Tasks

Setup XDEBUG in php that connects to vscode.
Find a way to intrgate ansible-playbook to do some task.

## Instructions

To complete this test.

1. Fork this repository
2. Fix the issues in docker-compose
3. Fix nginx
4. Fix apache/httpd
5. Add a database
6. Add php
7. Add adminer/phpmyadmin
8. Install Wordpress
9. Fix any permission issues (403)
10. Export the database to an sql file, make docker mariadb import the sql file on docker-compose up, you can use the docker-entrypoint-initdb.d folder for this. 
11. Create a pull request to this repository

The task is done, when you I (Lars) can clone the project and run docker-compose up and have a working wordpress solution, without having to go through to wordpress installer. You don't have to follow everything here head to toes. If you find different ways to solve the problems, feel free to do so.
