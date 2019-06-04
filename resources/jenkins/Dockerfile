FROM jenkins/jenkins:latest

MAINTAINER Mo Ahmed

ENV JAVA_OPTS="-Djenkins.install.runSetupWizard=false"
COPY plugins.txt $JENKINS_HOME/
RUN install-plugins.sh < $JENKINS_HOME/plugins.txt
RUN mkdir $JENKINS_HOME/builds

