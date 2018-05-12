From centos:6

MAINTAINER ug1y yinhao746746@163.com

RUN yum install -y openssh openssh-clients openssh-server telnet telnet-server
RUN yum install -y zsh gcc john vim nmap iptstate 
RUN yum install -y system-config-firewall xinetd wireshark hping3 squid

RUN useradd -m student
RUN echo password | passwd --stdin student
RUN useradd -m Instructor
RUN echo password | passwd --stdin Instructor

RUN service sshd start

CMD /bin/bash