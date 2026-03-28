FROM node:20
# This creates and moves to the directory
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO=true \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
    REDIS_URL="redis://redis:6379"
CMD ["node", "server.js"]