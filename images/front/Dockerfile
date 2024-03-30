FROM node:20-alpine

WORKDIR /app

ARG APP_PATH

COPY ${APP_PATH}/package*.json ./

RUN npm i

RUN npm i -g vite

COPY ${APP_PATH} /app

CMD npm i && npm start