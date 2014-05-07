FROM java

RUN wget -O /tmp/play-2.2.3.zip http://downloads.typesafe.com/play/2.2.3/play-2.2.3.zip
RUN yum -y install unzip
RUN unzip -d /opt/ /tmp/play-2.2.3.zip
RUN mv /opt/play-* /opt/play
RUN rm -f /tmp/play-2.2.3.zip

