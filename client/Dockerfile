FROM node:alpine as build

WORKDIR /app

COPY ./package.json ./
RUN npm install

COPY ./ ./

RUN npm run build

FROM nginx:latest as run

COPY ./config/nginx/default.conf /etc/nginx/conf.d/default.conf
COPY --from=build /app/build /etc/nginx/html

EXPOSE 3000