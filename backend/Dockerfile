FROM node:20
WORKDIR /opt/backend
COPY package.son .
copy *.js .
RUN npm install
ENV DB_HOST="mysql"
CMD ["node", "index.js"]