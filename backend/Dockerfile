# Use official Node.js LTS base image
FROM node:18-alpine

# Set working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port your app runs on (default: 3000)
EXPOSE 5000

# Start the Express server
CMD ["npm", "start"]
