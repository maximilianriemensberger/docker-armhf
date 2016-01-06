FROM maximilianriemensberger/armhf-base:latest
RUN \
	export DEBIAN_FRONTEND=noninteractive && \
	apt-get update && \
	apt-get install -q -y --no-install-recommends openjdk-8-jdk && \
	apt-get autoremove && \
	apt-get clean

RUN update-java-alternatives -s java-1.8.0-openjdk-armhf

ENV JAVA_HOME /usr/lib/jvm/java-1.8.0-openjdk-armhf

# vim: set noet tw=80 ts=8 sts=8 sw=8 :
