FROM centosFROM centos:latest
Author="venkatesh"
LABEL maintainer="venkateshpensalwar@gmail.com"
LABEL version="1.0"
RUN yum install openssh-server openssh-clients -y
RUN /usr/bin/ssh-keygen -A
RUN rm -rf /run/nologin
RUN echo "root:root" | chpasswd
CMD  ["/usr/sbin/sshd","-D"]
