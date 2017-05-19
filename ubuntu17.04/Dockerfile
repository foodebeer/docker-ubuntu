FROM ubuntu:17.04

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y apt-utils apt-transport-https ca-certificates curl software-properties-common
# Add Docker GPG key
RUN curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add -
# Add Docker repo
RUN add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) edge"
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y docker-ce=17.05.0~ce-0~ubuntu-zesty

CMD ["/bin/bash"]