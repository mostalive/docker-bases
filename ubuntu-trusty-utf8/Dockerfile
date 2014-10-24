# In case minimal debian is not enough - https://docs.docker.com/articles/dockerfile_best-practices/
FROM ubuntu:trusty

# Set the locale, otherwise we get invalid byte sequence errors
COPY locale.gen /etc/locale.gen
RUN locale-gen
ENV LANG en_US.UTF-8
ENV LANGUAGE en_US:en
ENV LC_ALL en_US.UTF-8

