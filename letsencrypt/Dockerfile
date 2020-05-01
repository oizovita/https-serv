FROM ubuntu:latest

RUN apt update \
    && sudo apt upgrade \
    && apt-get -y install software-properties-common \
    && add-apt-repository -y universe \
    && add-apt-repository -y ppa:certbot/certbot \
    && apt-get update \
    && apt-get -y install certbot \
    && apt-get -y install python-certbot-nginx

RUN certbot --nginx -d ${domain}



