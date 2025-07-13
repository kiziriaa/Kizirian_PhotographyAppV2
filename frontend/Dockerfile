# Use Node.js base image
FROM node:18-bullseye

# Create app directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the app
COPY . .

# Expose the Vite default port
EXPOSE 5173

# Start the dev server (hosted mode allows external access)
CMD ["npm", "run", "dev", "--", "--host"]
