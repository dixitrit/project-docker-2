# Use an official Node.js runtime as a base image
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app2

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install application dependencies
RUN npm install

# Copy the rest of the application source code to the container
COPY . .

# Expose the port your application listens on (e.g., 3000)
EXPOSE 3000

# Define the command to run your application
CMD ["node", "index.js"]
