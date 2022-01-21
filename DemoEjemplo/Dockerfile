FROM node:12-alpine
# Adding build tools to make yarn install work on Apple silicon / arm64 machines
RUN apk add --no-cache python2 g++ make
WORKDIR /app
COPY . .
EXPOSE 4500
RUN yarn install --production
CMD ["node", "src/server.15.02.js"]