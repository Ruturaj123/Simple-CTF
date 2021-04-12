FROM debian:jessie
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y --no-install-recommends wget unzip libc6-i386 libc6-dev-i386 default-jre default-jdk

COPY continuum.zip .
RUN unzip continuum.zip

RUN mv flag /home

EXPOSE 8080
CMD ["./apache-continuum-1.4.0/bin/continuum", "console"]