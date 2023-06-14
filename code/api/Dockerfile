FROM node:20.3-alpine
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run-script build:prod
EXPOSE 8000
CMD [ "node", "build/index.js" ]