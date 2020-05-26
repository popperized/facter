FROM node:current-slim
WORKDIR usr/src/app
ENV NPM_CONFIG_PREFIX /home/node/.npm-global
ENV PATH $PATH:/home/node/.npm-global/bin
USER node
RUN npm install -g hasura-cli
CMD ["hasura"]