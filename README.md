# For start
## Install docker
```sh
./ubuntu-docker-install.sh
```
or
```
https://docs.docker.com/engine/install/
```
## Clone project
```sh
git clone git@github.com:oizovita/https-serv.git
cd https-serv
```
## Setting docker
Replace oizovita@yahoo.com by your own email within the certificatesresolvers.myresolver.acme.email command line argument of the traefik service.

Replace www.oles.ninja by your own domain within the traefik.http.routers.whoami.rule label of the whoami service.
## Start server
```sh
docker-compose up -d
```
Open your domain
https://{domain}