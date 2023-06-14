FROM node:20.3-alpine
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run-script build:server:prod
EXPOSE 3000
CMD [ "npm", "run-script", "start:server:prod" ]