# base image
FROM node:alpine

WORKDIR /usr/app
# Install dependencies
COPY ./package.json ./
RUN npm install
COPY ./ ./

# Comand on startup
CMD ["npm","start"]