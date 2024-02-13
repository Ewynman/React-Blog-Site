# Base image
FROM node:17-alpine

# Directory Where commands will be run in
WORKDIR /app

# Copy Source code
# First dot is source of code
# Second dot is path within image where files go to
COPY . .

# Install Project Dependcies
RUN npm install

# Select a port number to expose so the app can make 
# request through the API
EXPOSE 4000

# Run the app
CMD ["node", "app.js"]