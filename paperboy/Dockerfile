FROM alpine
RUN apk add update --no-cache nodejs npm
RUN apk add yarn
WORKDIR /$(AppName)
COPY . /$(AppName)
RUN npm install yarn --global
CMD $(Debug) yarn run start
