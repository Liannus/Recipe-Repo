FROM node:10.16.3-alpine

RUN mkdir /frontend_container
WORKDIR /frontend_container

COPY package*.json ./
RUN npm install

COPY . .
RUN npm run build

EXPOSE 3000
