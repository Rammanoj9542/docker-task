FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json (if present)
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy application code
COPY index.js ./

# Expose port 3000
EXPOSE 3000

# Start the service
CMD ["npm", "run", "start"]
