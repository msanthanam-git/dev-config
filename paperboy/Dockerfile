FROM alpine
# RUN apk add --update npm
RUN apk add --no-cache --update nodejs npm
# RUN apk add --no-cache --update npm
RUN apk add nodejs-current
# RUN apk add yarn
WORKDIR /$(AppName)
COPY . /$(AppName)
# RUN npm install yarn --global
RUN npm install
CMD $(Debug) npm start
