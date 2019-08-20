FROM ppizzo/latex:debian

MAINTAINER Pietro Pizzo <pietro.pizzo@gmail.com>

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get -y install wget
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /usr/share/doc* /usr/share/man/* /usr/share/info/*
RUN wget -nv http://mirrors.ctan.org/macros/latex/contrib/europasscv.zip
RUN unzip europasscv.zip
RUN cp -a europasscv $(kpsewhich -var-value TEXMFDIST)/tex/latex
RUN rm -rf *
