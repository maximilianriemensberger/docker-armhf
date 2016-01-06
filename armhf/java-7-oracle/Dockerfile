FROM maximilianriemensberger/armhf-base:latest
RUN \
	echo debconf shared/accepted-oracle-license-v1-1 select true | \
		debconf-set-selections && \
	echo "deb http://ppa.launchpad.net/webupd8team/java/ubuntu wily main" >> \
		/etc/apt/sources.list && \
	apt-key adv --keyserver keyserver.ubuntu.com --recv-keys C2518248EEA14886 && \
	export DEBIAN_FRONTEND=noninteractive && \
	apt-get update && \
	apt-get install -q -y oracle-java7-installer oracle-java7-set-default && \
	apt-get autoremove && \
	apt-get clean

ENV JAVA_HOME /usr/lib/jvm/java-7-oracle

# vim: set noet tw=80 ts=8 sts=8 sw=8 :
