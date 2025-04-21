# Use Node.js 20 base image
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy and install dependencies
COPY package*.json ./
RUN npm install -f

# Copy the rest of the app code
COPY . .

# Optional: expose the backend port (update if different)
EXPOSE 8888

# Set environment
# ENV NODE_ENV=development

# Start the backend server
CMD ["npm", "run", "start"]
