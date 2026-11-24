#Uses node 18 alpine image as base image
FROM node:18-alpine
#sets working directory to /app
WORKDIR /app
# copies all json files to working directory
COPY package*.json ./
# installs dependencies
RUN npm install
# copies all files to working directory
COPY . .
#create directory for SQLite database file
RUN mkdir -p /app/data
#exposes port 5000 for application
EXPOSE 5000
#starts the application
CMD ["npm", "start"]

