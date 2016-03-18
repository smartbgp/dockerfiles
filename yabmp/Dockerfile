FROM python:2.7

MAINTAINER Peng Xiao <xiaoquwl@gmail.com>

RUN apt-get update

RUN apt-get install -y --no-install-recommends python-dev python-pip wget build-essential unzip

RUN wget https://github.com/smartbgp/yabmp/archive/master.zip

RUN unzip master.zip &&  \
    cd yabmp-master  && \
    pip install -r requirements.txt && \
    python setup.py install


EXPOSE 20000

ADD start.sh ./start.sh

VOLUME ["~/data"]

ENTRYPOINT ["./start.sh"]