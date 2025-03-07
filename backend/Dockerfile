# FROM node:20
FROM node:20.18.3-alpine3.21
RUN addgroup -S expense && adduser -S appuser -G appgroup
RUN mkdir /opt/backend
RUN chown -R expense:expense /opt/backend
WORKDIR /opt/backend
COPY package.json .
COPY  *.js .
RUN npm install
ENV DB_HOST="mysql"
# ENV DB_HOST="localhost"
USER expense
CMD ["node", "index.js"]

