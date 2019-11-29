FROM alpine
RUN apk add --update npm
RUN apk add nodejs-current
RUN apk add yarn
WORKDIR /$(AppName)
COPY . /$(AppName)
RUN npm install yarn --global
CMD $(Debug) yarn run start
