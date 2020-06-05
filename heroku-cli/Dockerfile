FROM node:current-slim
ARG CLI_VERSION=7.42.1
ARG LIB_VERSION=4.2.1
WORKDIR usr/src/app
RUN npm install -g heroku@${CLI_VERSION}
RUN apt install python3 python3-pip
RUN pip3 install heroku3==${LIB_VERSION}
CMD ["heroku"]
