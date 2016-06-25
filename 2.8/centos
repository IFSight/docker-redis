FROM fulcrum/centos7
MAINTAINER IF Fulcrum "fulcrum@ifsight.net"

RUN echo "Cache bust 201604291406" && \
    yum --noplugins install -y http://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-6.noarch.rpm && \
    yum --noplugins install -y redis && \
    yum --noplugins upgrade -y && \
    package-cleanup --dupes && \
    package-cleanup --cleandupes && \
    yum clean all

ENTRYPOINT ["/usr/bin/redis-server"]
CMD ["/etc/redis/redis.conf"]
