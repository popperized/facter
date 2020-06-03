FROM node:current-slim
WORKDIR usr/src/app
RUN npm install -g heroku
RUN apt install python3 python3-pip
RUN pip3 install heroku3
CMD ["heroku"]
