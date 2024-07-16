FROM node:20 AS build

WORKDIR /app

COPY package.json yarn.lock ./
RUN yarn install
COPY . ./

#RUN yarn run check
RUN yarn build

FROM node:20-slim

WORKDIR /app

COPY --from=build /app/package.json /app/yarn.lock ./

RUN yarn --prod

COPY .env ./
COPY --from=build /app/build .

CMD [ "node", "./index.js" ]
