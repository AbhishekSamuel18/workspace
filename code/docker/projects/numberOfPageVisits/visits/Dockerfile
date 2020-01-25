# base image
FROM node:alpine as builder

# install dependencies
WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .

FROM nginx
COPY --from=builder /app/build /usr/share/nginx