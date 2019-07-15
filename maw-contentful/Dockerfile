FROM alpine
RUN apk add --no-cache nodejs npm
WORKDIR /maw-contentful
COPY . /maw-contentful
RUN npm install
CMD npm start
