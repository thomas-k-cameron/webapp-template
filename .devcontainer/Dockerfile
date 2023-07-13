FROM mcr.microsoft.com/devcontainers/javascript-node:0-18
RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install git yarn

# install go lang
RUN  rm -rf /usr/local/go && tar -C /usr/local -xzf go1.20.6.linux-amd64.tar.gz && export PATH=$PATH:/usr/local/go/bin &&  echo "$(go version)"