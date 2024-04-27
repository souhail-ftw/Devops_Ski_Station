FROM jenkins/jenkins:lts

USER root

RUN apt-get update \
    && apt-get install -y default-jdk maven docker.io \
    && rm -rf /var/lib/apt/lists/*
RUN usermod -aG docker jenkins

USER jenkins
