

# Use Node.js Alpine image
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package configuration
COPY package*.json ./

# Install production dependencies
RUN npm install --omit=dev

# Copy application source code
COPY . .

# Run as non-root user
USER node

# Backend port
EXPOSE 3000

# Start backend application
CMD ["npm", "start"]
