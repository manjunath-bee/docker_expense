FROM node:20
WORKDIR /app
COPY *.js .
COPY package.json .
RUN npm install
ENV DB_HOST="mysql"
CMD ["node","index.js"]