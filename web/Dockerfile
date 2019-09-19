#Simple web server for test purposes
FROM ubuntu:18.04

LABEL version="1.0"
LABEL description="Simple web server image"
LABEL maintainer="Reysmer Valle <reysmerwvr@gmail.com>"

RUN apt-get update && apt-get install -y \ 
    apache2 \ 
    apache2-utils \
    nano \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

EXPOSE 80

ENTRYPOINT [ "apache2ctl" ]
CMD [ "-D", "FOREGROUND" ]
#CMD [ "apache2ctl", "-D", "FOREGROUND" ]