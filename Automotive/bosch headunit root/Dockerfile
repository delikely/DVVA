FROM ubuntu:12.04

WORKDIR /etc/

COPY ./udev.tar.gz /etc/

RUN tar xzvf udev.tar.gz -C ./udev/ 

CMD ["udevd"]

# 1. docker build -t delikely/bosch_headunit_root:automount .
# 2. docker run -itd --privileged=true --name bosch_headunit_root  delikely/bosch_headunit_root:automount
