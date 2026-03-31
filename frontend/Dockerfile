# frontend/Dockerfile
FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

# Set host to 0.0.0.0 so Docker port mapping works
ENV HOST=0.0.0.0
EXPOSE 3000

CMD ["npm", "start"]
