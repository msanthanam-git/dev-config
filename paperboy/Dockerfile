FROM node as build
WORKDIR /$(AppName)
COPY . /$(AppName)
RUN npm install

FROM gcr.io/distroless/nodejs
COPY --from=build /$(AppName) /
CMD $(Debug) npm start
