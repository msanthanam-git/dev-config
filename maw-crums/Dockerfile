FROM alpine
RUN apk add --no-cache nodejs npm
WORKDIR /maw-crums
COPY ${System.DefaultWorkingDirectory} /maw-crums
RUN npm install
CMD npm start
