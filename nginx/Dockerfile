FROM nginx:1.21
RUN apt-get update && apt-get install -y openssl
RUN mkdir -p /etc/nginx/ssl && mkdir -p /srv/data

COPY default.conf /etc/nginx/conf.d/
COPY start.sh /
ENTRYPOINT [ "/start.sh" ]
