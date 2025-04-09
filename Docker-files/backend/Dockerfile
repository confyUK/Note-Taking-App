# Step 1: Use the official Node.js image
FROM node:16-alpine

# Step 2: Set the working directory
WORKDIR /app

# Step 3: Copy the package.json and package-lock.json files
COPY package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy the rest of the application code
COPY . .

# Step 6: Expose the port the app will run on
EXPOSE 5000

# Step 7: Run the backend server
CMD ["npm", "start"]
