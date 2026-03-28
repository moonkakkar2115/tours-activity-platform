# Use Node.js LTS
FROM node:20

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy backend code
COPY . .

# Expose port (change if your backend uses another port)
EXPOSE 5000

# Start the backend
CMD ["npm", "start"]
