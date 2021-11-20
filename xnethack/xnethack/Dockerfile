#####
#
# xnethack on Ubuntu Desktop container
# 
#####
FROM dorowu/ubuntu-desktop-lxde-vnc
LABEL desc="for playing and testing xnethack on ubuntu desktop"
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
    bash \
    vim \
    games-rogue

# move to homedir
WORKDIR /root

# invoke root process
CMD ["/bin/bash"]
