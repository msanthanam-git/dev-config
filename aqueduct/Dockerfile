FROM alpine
ENV MONGODB_URI=$(MONGODB_URI)
ENV CRUMS_URL=$(CRUMS_URL)
ENV CRUMS_SCRIPT_TIME=$(CRUMS_SCRIPT_TIME) 
RUN apk add --no-cache nodejs npm
WORKDIR /$(AppName)
COPY . /$(AppName)
RUN npm install
CMD $(Debug) npm start
