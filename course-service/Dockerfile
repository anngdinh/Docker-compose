FROM node:10

# app directory
# WORKDIR /home/annd2/Documents/app/
# RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY ./package*.json ./

RUN npm install

COPY . .

# use 8080 in docker, not in local
EXPOSE 8080

CMD ["node", "index.js"]


# sudo docker build -t my-node-app:v0.0.7 .
# sudo docker run -p 5001:8080 my-node-app:v0.0.7