FROM node:16.20

RUN mkdir -p /usr/src/app
RUN mkdir -p /usr/src/app/backend

WORKDIR /usr/src/app/backend

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 9000

CMD ["npm","run","serve"]