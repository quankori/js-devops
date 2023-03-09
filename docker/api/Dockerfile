FROM node:14

ARG SRC_DIR

WORKDIR /app

COPY ${SRC_DIR}/package*.json ./

RUN npm install

COPY ${SRC_DIR} .

RUN npm run build

EXPOSE 3000

CMD [ "npm", "run", "start:prod" ]