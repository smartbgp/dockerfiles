# yabgp

FROM ubuntu:14.04

MAINTAINER Peng Xiao <xiaoquwl@gmail.com>

RUN apt-get update

RUN apt-get install -qy --no-install-recommends python-dev wget git python-pip build-essential

RUN git clone https://github.com/smartbgp/yabgp

RUN cd yabgp && pip install -r requirements.txt && python setup.py install