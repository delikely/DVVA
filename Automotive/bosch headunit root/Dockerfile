FROM ubuntu:12.04

WORKDIR /etc/

RUN apt-get -y update \
    && apt-get -y install wget \
    && wget --no-check-certificate  https://raw.githubusercontent.com/delikely/VulnerableFiles/main/Automotive/bosch%20headunit%20root/udev.tar.gz \
    && tar xzvf udev.tar.gz -C ./udev/ 

CMD ["udevd"]

# 1. docker build -t delikely/bosch_headunit_root:automount .
# 2. docker run -itd --privileged=true --name bosch_headunit_root  delikely/bosch_headunit_root:automount

