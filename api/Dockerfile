FROM node:17-alpine

WORKDIR /app

COPY package.json .

RUN yarn

COPY . .

EXPOSE 4000

CMD ["node", "app.js"]