FROM python:latest
RUN apt-get -y update --allow-releaseinfo-change && \
    apt-get -y upgrade

# install basics
RUN apt-get install -y git gcc python3-dev python3-pip zip file lsb-release telnet net-tools

# Viper and other binary Framework pre-reqs
RUN apt-get install -y libssl-dev swig libffi-dev ssdeep libfuzzy-dev unrar-free p7zip-full exiftool clamav-daemon libdpkg-perl

#RUN pip3 install viper-framework yara-python virustotal-api pyclamd  python-idb

# Windows Registry
RUN apt-get install -y registry-tools chntpw libhivex-bin 

# Analyse macros
RUN pip3 install oletools

# Install webtools
RUN apt-get install -y curl wget lynx  

# Install HexDump
RUN apt-get install -y xxd

# Install networking tshark
RUN apt-get install -y tshark


# Install Powershell
###################################

RUN wget https://github.com/PowerShell/PowerShell/releases/download/v7.3.9/powershell_7.3.9-1.deb_amd64.deb
RUN dpkg -i powershell_7.3.9-1.deb_amd64.deb
