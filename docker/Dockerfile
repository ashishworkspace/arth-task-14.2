FROM centos:latest
RUN yum install openssh-server -y
RUN echo "root:password" | chpasswd
RUN ssh-keygen -A
CMD ["/usr/sbin/sshd","-D"]
EXPOSE 22
EXPOSE 80



