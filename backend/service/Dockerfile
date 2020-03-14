FROM node:12.16-alpine as builder

USER root
WORKDIR /usr/src/app
COPY package.json /usr/src/app/package.json
RUN npm install
COPY . /usr/src/app
RUN npm run build

EXPOSE 80
CMD ["node", "dist/main.js"]