FROM python:latest
RUN apt-get -y update --allow-releaseinfo-change && \
    apt-get -y upgrade

# install basics
RUN apt-get install -y git gcc python3-dev python3-pip zip ltrace file

# Viper and other binary Framework pre-reqs
RUN apt-get install -y libssl-dev swig libffi-dev ssdeep libfuzzy-dev unrar-free p7zip-full exiftool clamav-daemon libdpkg-perl

RUN pip3 install viper-framework yara-python virustotal-api pyclamd lief python-idb

# Analyse macros
RUN pip3 install oletools

# Install webtools
RUN apt-get install -y curl wget lynx  
