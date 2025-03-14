FROM python:3.10-slim

Label author="Nico4dev" maintainer="discord blitz4dev"

RUN         apt update \
            && apt -y install git gcc g++ ca-certificates dnsutils curl iproute2 ffmpeg procps tmux \
            && useradd -m -d /home/container containe


user container
ENV USER=container home /home/container
WORKDIR /home/container

COPY ./entrypoint.sh /entrypoint.sh
CMD ["/bin/bash", "/entrypoint.sh"]
