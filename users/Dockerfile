# Use the official Node.js image as the base image
FROM node:18

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json ./
RUN npm install

# Copy all files to the working directory
COPY . .

# Expose the required port
EXPOSE 3003

# Command to run the application
CMD ["node", "server.js"]