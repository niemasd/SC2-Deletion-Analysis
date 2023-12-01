FROM ubuntu:20.04
RUN apt-get update -qq && apt-get upgrade -y -qq && \
    echo ttf-mscorefonts-installer msttcorefonts/accepted-mscorefonts-eula select true | debconf-set-selections && \
    rm ~/.cache/matplotlib -fr && \
    DEBIAN_FRONTEND=noninteractive TZ=Etc/UTC apt-get install -y -qq git python3 python3-pip ttf-mscorefonts-installer && \
    pip3 install notebook seaborn
