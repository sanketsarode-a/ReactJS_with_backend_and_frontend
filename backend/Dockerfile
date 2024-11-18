# Use the official Node.js image from Docker Hub
FROM node:18

# Set the working directory
WORKDIR /app

# Copy the package.json and package-lock.json files
COPY backend/package*.json ./

# Install backend dependencies
RUN npm install

# Copy the rest of the backend code
COPY backend/ .

# Expose the port that the backend will run on
EXPOSE 4000

# Run the backend server
CMD ["npm", "start"]
