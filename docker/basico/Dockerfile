FROM debian:buster-slim

LABEL maintainer="victor rivero"

ENV NGINX_VERSION=1.17.8-1~buster
RUN apt-get update && apt-get upgrade -y \
  && apt-get install --no-install-recommends --no-install-suggests -y \
    apt-transport-https \
    ca-certificates \
    curl \
    git \
    gnupg1 \
    gzip \
    net-tools

RUN apt-get autoremove -y && apt-get clean \
    && rm -f /etc/apt/sources.list.d/php.list \
    && rm -rf /var/lib/apt/lists/*

EXPOSE 443

CMD [ "sleep", "30" ]