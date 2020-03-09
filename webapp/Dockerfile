# base image
FROM node:alpine
# Create app directory
WORKDIR /app
# Install app dependencies
COPY package*.json ./

RUN npm install --silent
# Copy app source code
COPY . .

#Expose port and start application
CMD ["npm", "start"]