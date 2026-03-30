FROM node:18

WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy all source code
COPY . .

# Build frontend
RUN npm run build

# Expose port 80
EXPOSE 80

# Serve the built app
CMD ["npx", "serve", "-s", "build"]
