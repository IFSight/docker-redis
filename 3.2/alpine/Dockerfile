FROM redis:3.2-alpine
MAINTAINER IF Fulcrum "fulcrum@ifsight.net"

RUN apk update && apk upgrade

ENTRYPOINT ["docker-entrypoint.sh"]

EXPOSE 6379

CMD [ "/etc/redis/redis.conf" ]
