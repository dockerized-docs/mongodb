# dockerized-docs-mongodb

# What is it? #
Dockerzied MongoDB documentation for offline use.

# Image description #
- Base image: `python:2.7`
- The mongodb docs `master` branch is cloned and built using Giza (Sphinx Documentation Build Automation)
- Httpd server is installed
- Mongodb documentation directory (`/docs/build/master/html`) is linked to httpd `DocumentRoot` (`/var/www/html`)

# How to use this image #

```console
$ docker run -d genadipost/mongodb

```
You can test it by visiting http://container-ip:80
