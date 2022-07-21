FROM node:18.4.0-alpine

# Create app directory and use it as the working directory
RUN mkdir -p /srv/app/matheuspadilha/my-react-app
WORKDIR /srv/app/matheuspadilha/my-react-app

COPY package.json /srv/app/matheuspadilha/my-react-app
COPY package-lock.json /srv/app/matheuspadilha/my-react-app/

RUN npm install

RUN npm install cross-env

COPY . /srv/app/matheuspadilha/my-react-app

CMD [ "npm", "start" ]