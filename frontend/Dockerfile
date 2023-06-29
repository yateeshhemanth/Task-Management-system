# Use Node.js v14 as the base image
FROM node:20.3.1-bullseye-slim

# Create a new directory for the frontend app
RUN mkdir -p /usr/src/app/frontend
WORKDIR /usr/src/app/frontend

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install the app's dependencies
RUN npm install

# Copy the rest of the application files to the container
COPY . .

# Expose port 3000 for the app to run on
EXPOSE 3000

# Set the default command to start the app
CMD ["npm", "start"]
