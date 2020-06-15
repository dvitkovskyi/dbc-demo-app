FROM node:12.16.1 
ENV VUE_APP_BACKEND_URL='http://backend:3002/todos'
ENV DEV_SERVER_PORT='3003'
WORKDIR /opt/front-end
COPY . /opt/front-end
RUN npm ci
RUN npm run lint && npm run build
EXPOSE 3003
CMD [ "npm", "run", "serve" ]
