# use an existing docker image as base

FROM alpine

# Download and install a dependency

RUN apk add --update redis
RUN apk add --update gcc

# Tell that image what to do when it starts as a container

CMD ["redis-server"]