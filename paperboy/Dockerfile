FROM alpine
RUN apk add --no-cache nodejs npm
#WORKDIR /$(AppName)
WORKDIR /paperboy
#COPY . /$(AppName)
COPY . /paperboy
RUN npm install
CMD $(Debug) npm start
