# Step 1: Use a Node.js base image
FROM node:18-alpine

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy package.json and package-lock.json (if available) into the working directory
COPY package*.json ./

# Step 4: Install application dependencies
RUN npm install

# Step 5: Copy the rest of the application code
COPY . .

# Step 6: Expose the application's port
EXPOSE 3000

# Step 7: Define the command to run the application
CMD ["npm", "start"]
