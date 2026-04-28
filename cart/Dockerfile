FROM node:20
WORKDIR /app
EXPOSE 8080
COPY server.js /app
COPY package.json /app
RUN npm install
ENV REDIS_HOST="redis" \
    CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080"
CMD ["node", "server.js"]
