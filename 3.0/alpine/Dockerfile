FROM redis:3.0-alpine
MAINTAINER IF Fulcrum "fulcrum@ifsight.net"

RUN echo "Cache bust 201606232004" && \
    apk update && apk upgrade

ENTRYPOINT ["docker-entrypoint.sh"]

EXPOSE 6379

CMD [ "/etc/redis/redis.conf" ]
