FROM ubuntu:22.04

RUN apt-get update

RUN apt-get install -y python3-pip && \
    pip3 install --upgrade pip && \
    pip3 install awscli

RUN pip3 install ansible

RUN apt-get install -y openssh-server openssh-client
    
RUN mkdir -p -m 755 /var/run/sshd

RUN mkdir -m 755 /root/.ssh

CMD /usr/sbin/sshd -D