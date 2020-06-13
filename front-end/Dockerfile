FROM node:latest
WORKDIR /usr/app
COPY . /usr/app
ENV VUE_APP_BACKEND_URL='http://backend:3002/todos'
ENV DEV_SERVER_PORT='3003'
RUN npm ci
RUN npm run lint && npm run build
EXPOSE 3003
CMD [ "npm", "run", "serve" ]
