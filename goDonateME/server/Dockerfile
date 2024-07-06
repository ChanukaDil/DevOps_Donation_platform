# Use an official Node.js image as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the backend code to the working directory
COPY . .

# Expose the application port
EXPOSE 8000

# Command to run the application
CMD ["npm", "run", "start"]
