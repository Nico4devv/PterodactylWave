FROM python:3.11-slim

LABEL author="Nico4dev" maintainer="discord blitz4dev"

RUN apt update \
    && apt -y install git gcc g++ ca-certificates dnsutils curl iproute2 ffmpeg procps tmux \
    && useradd -m -d /home/container container

USER container
ENV USER=container HOME=/home/container
WORKDIR /home/container

COPY ./entrypoint.sh /entrypoint.sh
CMD ["/bin/bash", "/entrypoint.sh"]
