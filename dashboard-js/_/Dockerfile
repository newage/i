FROM ubuntu:trusty

RUN apt-get update -y
RUN apt-get install -y git
RUN apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup | sudo -E bash -
RUN apt-get install -y nodejs
RUN npm install -g grunt-cli
RUN npm install -g bower &&\
    echo '{ "allow_root": true }' > /root/.bowerrc
RUN npm install -g grunt

RUN mkdir /opt/igov
WORKDIR /opt/igov

# ports join
EXPOSE 9001 1337
CMD ["bash"]
