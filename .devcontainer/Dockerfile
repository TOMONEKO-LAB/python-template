FROM python:3.12-slim


RUN apt-get update && apt-get -y install --no-install-recommends default-libmysqlclient-dev build-essential ca-certificates


RUN openssl x509 -inform der -in IIJ1.der -outform pem -out IIJ1.crt


RUN cp IIJ1.crt /usr/local/share/ca-certificates


RUN update-ca-certificates
