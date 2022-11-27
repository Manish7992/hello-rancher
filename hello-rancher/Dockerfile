FROM node:14.15.0 AS builder

# set working directory
WORKDIR /app


# install app dependencies
#copies package.json and package-lock.json to Docker environment
COPY package*.json ./

# Installs all node packages
RUN npm install


# Copies everything over to Docker environment
COPY . ./
CMD npm start
