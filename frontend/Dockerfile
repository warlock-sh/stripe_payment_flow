# Build stage
FROM node:24-alpine as build

WORKDIR /app

# Install dependencies
COPY package.json package-lock.json* ./
RUN npm install

# Copy application code
COPY . .

# Build the application
# RUN npm run build

# Expose port
EXPOSE 8080

# Start the application
CMD ["npm", "run", "dev"] 