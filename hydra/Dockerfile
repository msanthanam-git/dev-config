FROM alpine
RUN apk add --no-cache nodejs npm
WORKDIR /hydra
COPY . /hydra
RUN npm install
EXPOSE 3000
CMD npm start
