ARG BUILD_FROM
FROM $BUILD_FROM

ENV LANG C.UTF-8

RUN apk add haproxy
ADD https://github.com/hassio-addons/bashio/archive/v0.14.3.tar.gz /tmp/bashio.tar.gz

COPY run.sh haproxy.cfg /

RUN chmod a+x /run.sh
CMD [ "/run.sh" ]
