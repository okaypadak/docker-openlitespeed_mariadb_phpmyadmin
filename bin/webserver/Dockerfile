FROM litespeedtech/openlitespeed:1.6.9-lsphp74

# Update and upgrade linux container
RUN apt-get -y update
RUN apt-get upgrade -y

# Install useful tools
RUN apt-get -y install apt-utils nano wget

# Install important libraries
RUN apt-get -y install --fix-missing apt-utils build-essential git curl libcurl4 zip openssl

# Install python3
RUN apt-get install -y python3-pip python3-dev \
    && cd /usr/local/bin \
    && ln -s /usr/bin/python3 python

# Autoremove unnecessary tools
RUN apt-get autoremove -y
