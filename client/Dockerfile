FROM node:20.11

WORKDIR /app

COPY package.json .

RUN apt-get update && apt-get install -y yarn

RUN yarn install

COPY . .

EXPOSE 3000

CMD ["yarn", "dev"]
