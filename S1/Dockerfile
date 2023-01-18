FROM node:14

# Each container has own working directory
WORKDIR /app

# Copy package.json to the root of container.
COPY package.json .

RUN npm install

# Copy other files to the root of container.
COPY . .

# Specify the exposed port (Depend on the implementation)
EXPOSE 3000

# Run command
CMD [ "node", "app.mjs"]