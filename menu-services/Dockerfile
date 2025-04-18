# Use Node.js as the base image
FROM node:18-alpine

# Set working directory
WORKDIR ./app

# Copy package.json and package-lock.json (if exists)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the source code
COPY . .

# Expose the port the API Gateway runs on
EXPOSE 3003

# Command to start the API Gateway
CMD ["node", "index.js"]