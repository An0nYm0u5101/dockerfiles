FROM python:3.12.4-alpine3.20
RUN pip install wsgidav cheroot
RUN mkdir -p /webdav/share && mkdir -p /srv/data/share
COPY run.sh /webdav/
WORKDIR /webdav/
ENTRYPOINT "/webdav/run.sh"
