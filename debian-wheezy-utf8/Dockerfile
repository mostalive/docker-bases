#Base off the latest debian release - https://docs.docker.com/articles/dockerfile_best-practices/
# https://registry.hub.docker.com/_/debian/
FROM debian:wheezy

# Set the locale, otherwise we get invalid byte sequence errors
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y \
    locales
COPY locale.gen /etc/locale.gen
RUN locale-gen
ENV LANG en_US.UTF-8
ENV LANGUAGE en_US:en
ENV LC_ALL en_US.UTF-8

