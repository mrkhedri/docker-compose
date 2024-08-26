ARG NIFI_VERSION

FROM apache/nifi:${NIFI_VERSION}
USER root
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    nano \
    mdbtools
RUN set -x \
    && sed -i 's/^deb\ http:\/\/deb.debian.org\/debian\ bullseye\ main.*$/deb\ http:\/\/deb.debian.org\/debian\ bullseye\ main\ contrib\ non-free/g' /etc/apt/sources.list \
    && apt-get update \
    && apt-get install -y unrar
USER nifi
