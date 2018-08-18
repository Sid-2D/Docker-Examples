FROM ubuntu:14.04

WORKDIR /server

ADD . /server

RUN	apt-get update -yq && apt-get upgrade -yq && \
	apt-get install -yq curl git nano && \
	curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash - && \
	sudo apt-get install -y nodejs && \
	sudo apt-get install -y build-essential && \
	npm install

EXPOSE 3000

ENV PORT 3000

CMD ["node", "server.js"]