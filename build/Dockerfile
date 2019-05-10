FROM node:10.15.3-alpine AS build-env
WORKDIR /usr/src/app
RUN apk update && apk --no-cache add git
RUN git clone https://github.com/cubedro/eth-net-intelligence-api.git .
RUN rm -rf .git
RUN npm install --production

FROM node:10.15.3-alpine
WORKDIR /usr/app
COPY --from=build-env /usr/src/app .
CMD [ "node", "app.js" ]