FROM openjdk:8


RUN apt-get -y update
RUN apt-get -y install apt-transport-https
RUN echo "deb https://dl.bintray.com/rundeck/rundeck-deb /" | tee -a /etc/apt/sources.list
RUN curl "https://bintray.com/user/downloadSubjectPublicKey?username=bintray" > /tmp/bintray.gpg.key
RUN apt-key add - < /tmp/bintray.gpg.key
RUN apt-get -y update
RUN apt-get -y install rundeck-cli