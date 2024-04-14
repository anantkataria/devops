# source : https://www.youtube.com/watch?v=pg19Z8LL06w

# base image which has linux application layer and node runtime pre-installed in it
FROM node:19-alpine

#copy code from local storage to isolated container
COPY package*.json /usr/app/
COPY src /usr/app/

# change current directory to run next commands in specified directory
WORKDIR /usr/app

# install app dependencies
RUN npm install

# final command that actually starts the application inside the container env
CMD ["node", "server.js"]