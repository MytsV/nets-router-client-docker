FROM ubuntu:impish

RUN apt-get update

RUN apt-get -y install iproute2 iputils-ping frr vim isc-dhcp-server

RUN apt update && apt install isc-dhcp-server sudo -y
RUN useradd -rm -d /home/router -s /bin/bash -g root -G sudo -u 1001 router
RUN echo "router:pass" | chpasswd