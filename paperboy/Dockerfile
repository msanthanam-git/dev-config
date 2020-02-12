#FROM alpine
#RUN apk add --no-cache nodejs npm
#WORKDIR /$(AppName)
#COPY . /$(AppName)
#RUN npm install
# FROM alpine
FROM node:latest
ARG NPM_TOKEN
COPY .npmrc .npmrc
#RUN apk update
#RUN apk add npm
#RUN apk add nodejs-current
# RUN apk add yarn
WORKDIR /$(AppName)
COPY . /$(AppName)
# RUN yarn upgrade
RUN yarn install
RUN rm -f .npmrc
# CMD $(Debug) npm start
# CMD $(Debug) npm dev
# CMD npx nodemon -e marko app.js
# CMD NODE_ENV=development node app.js
# CMD NODE_ENV=$(NODE_ENV) npx nodemon -e marko app.js
CMD NODE_ENV=$(NODE_ENV) npm start 
