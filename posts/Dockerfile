# posts/Dockerfile
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json from the root of the project (use the correct path)
COPY ../package.json ./
COPY ../package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of your application files
COPY ../ ./

# Expose the port your application is running on
EXPOSE 3000

# Command to run your app
CMD ["node", "server.js"]
