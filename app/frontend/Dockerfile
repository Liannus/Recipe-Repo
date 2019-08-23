FROM node:10.16.3-alpine

RUN mkdir -p /frontend
WORKDIR /frontend

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 3000
