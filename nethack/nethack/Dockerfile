#####
#
# nethack 3.6.0 on Ubuntu container
# ref https://zoomadmin.com/HowToInstall/UbuntuPackage/games-rogue
#
#####
FROM ubuntu:18.04
LABEL desc="for playing and testing nethack on ubuntu"
LABEL creator="ino9oni"

# timezone setting
#RUN apt-get update -y && apt-get install -y tzdata
#ENV TZ=Asia/Tokyo
#ENV LANG=en_US.UTF-8

# to change noninteractive
ENV DEBIAN_FRONTEND noninteractive
# to set path for nethack exec
ENV PATH $PATH:/usr/games

# to change root user
USER root

# install basic commands
RUN apt-get update -y && apt-get install -y \
#    hearse \
    bash \
    vim \
    games-rogue

# move to homedir
WORKDIR /root

# invoke root process
CMD ["/bin/bash"]
