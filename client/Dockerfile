FROM node:alpine

ENV CI=true

WORKDIR /app
COPY package.json ./
RUN npm install yarn
RUN yarn
RUN yarn add @babel/runtime

COPY ./ ./

CMD [ "yarn", "start" ]
