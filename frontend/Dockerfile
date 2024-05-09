# Use an official Node.js runtime as a base image
FROM node:18.16.0

# Set the working directory in the container
WORKDIR /app/frontend

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install frontend dependencies
RUN npm install

# Copy the frontend application code to the container
COPY . .

# Expose the port on which your frontend application is running
EXPOSE 3000

# Define the command to start your frontend application
CMD ["npm", "start"]
