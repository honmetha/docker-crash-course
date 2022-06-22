FROM node:17-alpine

RUN yarn global add nodemon

WORKDIR /app

COPY package.json .

RUN yarn

COPY . .

EXPOSE 4000

CMD ["yarn", "run", "dev"]