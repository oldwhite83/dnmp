ARG NODE_VERSION
FROM ${NODE_VERSION}

ARG TZ

# Create app directory
RUN mkdir -p /mnt/app
WORKDIR /mnt/app
RUN npm install --registry=https://registry.npm.taobao.org


RUN apk --no-cache add tzdata \
    && cp "/usr/share/zoneinfo/$TZ" /etc/localtime \
    && echo "$TZ" > /etc/timezone
