# The base image `node` is from Dockerhub.
# So, it's gonna start with `node` image.
FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

# COPY [PATH_IN_LOCAL] to [PATH_IN_CONTAINER]
COPY . /app

EXPOSE 80

# RUN: For running in the image inside the container
# CMD: For running in the host. (When container start to run.)
CMD ["node", "server.js"]