FROM ubuntu:22.04

RUN apt-get update

RUN apt-get install -y openssh-server openssh-client
    
RUN mkdir -p -m 755 /var/run/sshd

RUN mkdir -m 755 /root/.ssh

RUN apt-get install -y curl

CMD /usr/sbin/sshd -D 