FROM python:2.7.14-alpine

LABEL maintainer="Peng Xiao <xiaoquwl@gmail.com>"

ENV YABGP_VERSION 0.4.0

RUN apk add --no-cache gcc musl-dev && pip install yabgp==${YABGP_VERSION} && apk del gcc musl-dev

EXPOSE 8801

VOLUME ["~/data"]

ENTRYPOINT ["/usr/local/bin/yabgpd"]

CMD []