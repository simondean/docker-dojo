FROM play

#VOLUME /build/output/
#RUN rpm -Uvh http://www.mirrorservice.org/sites/dl.fedoraproject.org/pub/epel/6/i386/epel-release-6-8.noarch.rpm
#RUN yum -y install docker-io
RUN yum -y install unzip
WORKDIR /opt/play/samples/java/helloworld/
RUN echo -e "FROM java\nADD output/app/ /opt/app/\nWORKDIR /opt/app/\nENTRYPOINT bin/helloworld" > Dockerfile
#RUN ls -la
ENTRYPOINT ../../../play dist && mkdir -p output/app/ && unzip -d output/app/ -q target/universal/helloworld-*.zip && mv output/app/helloworld*/* output/app/ && rmdir output/app/helloworld*/ && docker build -t play-sample-app . 
