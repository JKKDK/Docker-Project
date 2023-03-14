FROM almalinux:latest

EXPOSE 8080/tcp

RUN yum update && \
    yum install nginx -y  && \
    yum install git -y

#  To reduce the number of layers and keep the image size small.

CMD ["nginx", "-g", "daemon off;"]

# to run the main process in the foreground to ensure that the container remains active and responsive

LABEL STUDENT="JKKDK" \
      AUTHOR="SHIVA" \
      CONTENT="DOCKER"

ENV AUTHOR="SHIVAKUMAR"\
    DURATION="6MONTHS"\
    CONTENT="DOCKER"

RUN rm -rf usr/share/nginx/html/index.html
COPY qi usr/share/nginx/html