# Base image
FROM node:17-alpine

# Directory Where commands will be run in
WORKDIR /app

# Install Project Dependcies
COPY package.json .
RUN npm install

# Copy Source code
# First dot is source of code
# Second dot is path within image where files go to
COPY . .

# Select a port number to expose so the app can make 
# request through the API
EXPOSE 4000

# Run the app
CMD ["node", "app.js"]