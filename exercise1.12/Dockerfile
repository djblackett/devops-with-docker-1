FROM node:16

WORKDIR /usr/src/app

COPY . /usr/src/app


ENV REACT_APP_BACKEND_URL=http://localhost:8080

RUN npm install



CMD ["npm", "run", "start"]
