#Download base image ubuntu 18.04
FROM ubuntu:18.04

# Update Software repository
RUN apt-get update

# Install python from ubuntu repository
RUN apt-get install -y git python python-pip python-virtualenv phantomjs nano vim xvfb

# Get repo. Thank to the author of this tool!
RUN git clone https://github.com/maaaaz/webscreenshot
RUN echo "Config is in the js file, change user-agent or resolution if you need" > webscreenshot/RUNME_manually.txt
RUN echo "Enter every command manually to enable headless OS." >> webscreenshot/RUNME_manually.txt
RUN echo "################################################################################" >> webscreenshot/RUNME_manually.txt
RUN echo "export DISPLAY=':99.0'" >> webscreenshot/RUNME_manually.txt
RUN echo "Xvfb :99 -screen 0 1024x768x24 > /dev/null 2>&1 &" >> /webscreenshot/RUNME_manually.txt
RUN touch webscreenshot/list.txt
