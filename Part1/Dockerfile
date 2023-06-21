FROM node:16.17.1-alpine3.15

WORKDIR /front-end

EXPOSE 5000

COPY . .

RUN npm install

RUN npm run build

RUN npm install -g serve

ENTRYPOINT ["serve", "-s", "-l", "5000", "build"]