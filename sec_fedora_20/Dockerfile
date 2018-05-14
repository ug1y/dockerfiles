From fedora:20

MAINTAINER ug1y yinhao746746@163.com

RUN yum install -y openssh openssh-clients telnet zsh gcc
RUN yum install -y mlocate john vim nmap hping3 wireshark

RUN echo password | passwd --stdin root
RUN useradd -m student
RUN echo password | passwd --stdin student
RUN useradd -m Instructor
RUN echo password | passwd --stdin Instructor

CMD /bin/bash