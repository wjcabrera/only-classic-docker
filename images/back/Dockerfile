FROM node:20-alpine

WORKDIR /app

ARG APP_PATH

COPY ${APP_PATH}/package*.json ./

RUN npm i

RUN npm i -g @nestjs/cli

COPY ${APP_PATH} /app

# RUN npm run build

CMD npm i && npm run start:dev