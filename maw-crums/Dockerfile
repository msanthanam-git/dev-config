FROM alpine
RUN apk add --no-cache nodejs npm
WORKDIR /maw-crums
COPY /home/vsts/work/1/s/uosdev/maw-crums/* /maw-crums
RUN npm install
CMD npm start
