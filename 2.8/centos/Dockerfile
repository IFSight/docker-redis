FROM fulcrum/centos7
MAINTAINER IF Fulcrum "fulcrum@ifsight.net"

RUN yum --noplugins install -y http://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-7.noarch.rpm && \
    yum --noplugins install -y redis && \
    yum --noplugins upgrade -y && \
    package-cleanup --dupes && \
    package-cleanup --cleandupes && \
    yum clean all

ENTRYPOINT ["/usr/bin/redis-server"]
CMD ["/etc/redis/redis.conf"]
