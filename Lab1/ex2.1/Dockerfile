FROM node:14.13.0-stretch

COPY package.json ./

RUN npm install

COPY server.js /usr/src/app/

EXPOSE 8080

CMD ["node", "/usr/src/app/server.js"]


