FROM alpine
RUN apk add --no-cache nodejs npm
WORKDIR /maw-entry
COPY . /maw-entry
RUN npm install
CMD npm start
