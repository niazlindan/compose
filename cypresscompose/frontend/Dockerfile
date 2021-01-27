FROM ubuntu:focal

RUN     apt update &&\
    apt install -y curl &&\
    curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh &&\
    bash nodesource_setup.sh &&\
    apt install -y nodejs


RUN npm install -g github-files-fetcher

RUN fetcher --url=https://github.com/niazlindan/realword/tree/main/realworld/frontend

RUN cd frontend && \
    npm install 