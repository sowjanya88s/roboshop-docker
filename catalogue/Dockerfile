FROM node:20
WORKDIR /app
COPY server.js /app
COPY package.json /app
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node", "server.js"]
