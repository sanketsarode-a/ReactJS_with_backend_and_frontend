# Use the official Node.js image from Docker Hub
FROM node:18

# Set the working directory
WORKDIR /app

# Copy the package.json and package-lock.json files
COPY frontend/package*.json ./

# Install frontend dependencies
RUN npm install

# Copy the rest of the frontend code
COPY frontend/ .

# Expose the port for the React app
EXPOSE 3000

# Run the frontend application
CMD ["npm", "start"]
