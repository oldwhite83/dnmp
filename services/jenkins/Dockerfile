FROM jenkins/jenkins:lts
USER root
# you can install docker-compose by curl; you also use existed docker-compose
# I use existed docker-compose
# RUN curl -L https://github.com/docker/compose/releases/download/1.25.0-rc1/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
COPY ./docker-compose /usr/local/bin/docker-compose
RUN  chmod +x /usr/local/bin/docker-compose
# remove cache for get smaller image
RUN  rm -rf /var/lib/apt/lists/*
