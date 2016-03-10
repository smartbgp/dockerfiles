FROM python:2.7

MAINTAINER Peng Xiao <xiaoquwl@gmail.com>

RUN apt-get update

RUN apt-get install -y --no-install-recommends python-dev python-pip wget build-essential unzip

RUN wget https://github.com/smartbgp/yabgp/archive/master.zip

RUN unzip master.zip &&  \
    cd yabgp-master  && \
    pip install -r requirements.txt && \
    python setup.py install


EXPOSE 8801

ADD start.sh ./start.sh

VOLUME ["~/data"]

ENTRYPOINT ["./start.sh"]