From i386/centos:6

MAINTAINER ug1y yinhao746746@163.com

RUN yum install -y openssh openssh-clients openssh-server telnet telnet-server zsh
RUN yum install -y gcc gdb vim iptstate system-config-firewall wireshark squid

RUN echo password | passwd --stdin root
RUN useradd -m student
RUN echo password | passwd --stdin student
RUN useradd -m Instructor
RUN echo password | passwd --stdin Instructor

RUN service sshd start

CMD /bin/bash