# Use an official Node.js runtime as a parent image
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files to the working directory
COPY . .

# Build the application for production
RUN npm run build

# Expose the port on which the app runs
EXPOSE 80

# Command to start the application
CMD ["npm", "run", "preview"]
