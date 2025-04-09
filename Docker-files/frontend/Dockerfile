# Step 1: Build Stage
FROM node:16-alpine AS build

# Set working directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy the app source code
COPY . .

# Build the app for production
RUN npm run build

# Step 2: Serve Stage
FROM nginx:alpine

# Copy the build files from the previous stage
COPY --from=build /app/build /usr/share/nginx/html

# Expose the port for the React app
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]
