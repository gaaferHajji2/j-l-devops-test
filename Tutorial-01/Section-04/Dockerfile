FROM node:14.16.0-alpine3.13
RUN addgroup app && adduser -S -G app app
USER app
WORKDIR /app
COPY package*.json .
RUN ["npm", "i"]
RUN ["mkdir", "data"]
COPY . .
ENV API_URL=https://jafar.loka.com/
EXPOSE 3000
# Exec Form
# CMD [ "npm", "i", "&&" ,"npm", "start"]
CMD ["npm", "start"]
