# Use Jenkins LTS as the base image
FROM jenkins/jenkins:lts

# Switch to root user to install dependencies
USER root

# Install OpenJDK 11 and Maven
RUN apt-get update \
    && apt-get install -y default-jdk maven \
    && rm -rf /var/lib/apt/lists/*

# Switch back to the Jenkins user
USER jenkins
