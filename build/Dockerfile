FROM play

RUN yum -y install unzip
ADD ./Dockerfile_app /opt/play/samples/java/helloworld/
ADD ./build_app /opt/play/samples/java/helloworld/
WORKDIR /opt/play/samples/java/helloworld/
ENTRYPOINT ./build_app
EXPOSE 9000
