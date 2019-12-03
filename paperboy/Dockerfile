#FROM alpine
#RUN apk add --no-cache nodejs npm
#WORKDIR /$(AppName)
#COPY . /$(AppName)
#RUN npm install
FROM alpine
ARG NPM_TOKEN
COPY .npmrc .npmrc
RUN apk update
RUN apk add npm
RUN apk add nodejs-current
RUN apk add yarn
WORKDIR /$(AppName)
COPY . /$(AppName)
RUN yarn upgrade
RUN yarn install
RUN rm -f .npmrc
CMD $(Debug) npm start
