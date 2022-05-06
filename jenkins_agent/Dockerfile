FROM jenkins/ssh-agent:4.2.1-jdk11

RUN apt-get update \
&& apt-get install -y git curl python3 python3-pip \
&& groupadd docker \
&& usermod -aG docker jenkins

RUN curl -fsSL https://get.docker.com | sh 