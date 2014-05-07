FROM centos

RUN yum -y install wget
RUN wget --no-cookies --no-check-certificate --header "Cookie: gpw_e24=http%3A%2F%2Fwww.oracle.com%2F; oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/7u55-b13/jdk-7u55-linux-x64.rpm -O /tmp/jdk-7u55-linux-x64.rpm; yum -y install /tmp/jdk-7u55-linux-x64.rpm; rm -f /tmp/jdk-7u55-linux-x64.rpm

