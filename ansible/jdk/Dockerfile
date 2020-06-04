FROM ubuntu:18.04

# Install Java.
RUN \
#   echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections && \
#   add-apt-repository -y ppa:webupd8team/java && \
  apt-get update && \
  apt-get install -y openjdk-8-jdk
#   DEBIAN_FRONTEND=noninteractive apt install software-properties-common && \
#   DEBIAN_FRONTEND=noninteractive add-apt-repository ppa:linuxuprising/java && \
#   DEBIAN_FRONTEND=noninteractive apt-get update && \
#   DEBIAN_FRONTEND=noninteractive apt install oracle-java11-installer 
#   rm -rf /var/lib/apt/lists/* && \
#   rm -rf /var/cache/oracle-jdk8-installer


# Define working directory.
WORKDIR /data

# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-11-openjdk-amd64

# Define default command.
CMD ["bash"]