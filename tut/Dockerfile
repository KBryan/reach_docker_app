FROM node:14.16.0-alpine3.13

# RUN addgroup app && adduser -S -G app app

# USER app

WORKDIR /app

COPY package*.json .

RUN npm install

COPY . .

RUN npm install

ENV API_URL=http://api.test.com

EXPOSE 3000

CMD ["./reach", "react"]

