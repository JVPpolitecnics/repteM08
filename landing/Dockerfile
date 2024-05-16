# Use a Node.js base image with a specified version
FROM node:latest

# Set working directory inside the container
WORKDIR /var/www

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all project files to the working directory
COPY . .

# Expose port 3000 (the default port Vite runs on)
EXPOSE 3000

# Command to run the development server
CMD ["npm", "run", "dev"]
