#FROM node:20
FROM node:alpine3.20
RUN addgroup -S expense && adduser -S expense -G expense && \
    mkdir /app && \
    chown -R expense:expense /app
WORKDIR /app
ENV DB_HOST="mysql"
USER expense
CMD ["node","index.js"]
COPY *.js ./
COPY package.json ./
RUN npm install
# ENV DB_HOST="mysql"
# USER expense
# CMD ["node","index.js"]