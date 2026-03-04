FROM node:20.0
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO_URL="mongodb://mongodb:27017/users" \
    REDIS_URL="redis://redis:6379" \
    MONGO=true
CMD ["node","server.js"]    