FROM node:14.16.0-alpine3.13
WORKDIR /app
COPY . .
RUN npm i
ENV API_URL=https://jafar.loka.com/
EXPOSE 3000
RUN addgroup app && adduser -S -G app app
USER app
