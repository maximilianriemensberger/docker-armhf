FROM armv7/armhf-ubuntu
MAINTAINER Maximilian Riemensberger <maximilian.riemensberger@gmail.com>

RUN export DEBIAN_FRONTEND=noninteractive && \
	apt-get update && \
	apt-get install -y apt-utils && \
	apt-get upgrade -y && \
	apt-get autoremove && \
	apt-get clean

RUN export DEBIAN_FRONTEND=noninteractive && \
	apt-get install -y \
		bash \
		bash-completion \
		bzip2 \
		ca-certificates \
		curl \
		file \
		gawk \
		git \
		grep \
		gzip \
		jq \
		less \
		libcurl4-openssl-dev \
		libssl-dev \
		passwd \
		python \
		rsync \
		sed \
		ssh-client \
		tar \
		unzip \
		vim \
		wget \
		xz-utils \
		zip \
	&& \
	apt-get autoremove && \
	apt-get clean

RUN export DEBIAN_FRONTEND=noninteractive && \
	apt-get install -y \
		autoconf \
		autogen \
		automake \
		binutils \
		build-essential \
		gcc \
		g++ \
		libtool \
		make \
		pkg-config \
	&& \
	apt-get autoremove && \
	apt-get clean

CMD ["/bin/bash"]

# vim: set noet tw=80 ts=8 sts=8 sw=8 :
