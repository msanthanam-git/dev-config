FROM alpine
RUN apk add --no-cache nodejs npm
WORKDIR /$(AppName)
COPY . /$(AppName)
RUN npm install
CMD $(Debug) npm start
