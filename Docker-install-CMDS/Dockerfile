FROM almalinux:latest

EXPOSE 8080/tcp

RUN yum update -y && \
    yum install nginx -y  && \
    yum install git -y

#  To reduce the number of layers and keep the image size small.

# CMD ["nginx", "-g", "daemon off;"]

# to run the main process in the foreground to ensure that the container remains active and responsive

LABEL STUDENT="JKKDK" \
      AUTHOR="SHIVA" \
      CONTENT="DOCKER"

ENV AUTHOR="SHIVAKUMAR"\
    DURATION="6MONTHS"\
    CONTENT="DOCKER"

RUN rm -rf usr/share/nginx/html/index.html
COPY qi usr/share/nginx/html

ADD https://raw.githubusercontent.com/TechPrimers/jenkins-example/master/pom.xml /tmp 
ADD apache-tomcat-9.0.73-embed.tar.gz /tmp

CMD ["ping", "-c5", "google.com"]

ENTRYPOINT ["ping", "-c5", "google.com"]
# appending the arguments passed throgh commandline



