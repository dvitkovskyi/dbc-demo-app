FROM node:12.16.1 as frontend
ENV VUE_APP_BACKEND_URL=http://backend:3002/todos
ENV DEV_SERVER_PORT='3002'
WORKDIR /demo/front-end
COPY ./package*.json /demo/front-end/
RUN npm ci
COPY . /demo/front-end/
RUN npm run lint && npm run build
EXPOSE 3003
CMD [ "npm", "run", "serve" ]
