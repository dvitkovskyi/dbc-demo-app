FROM node:12.16.1 as backend
ENV MONGO_URI='mongodb://mongo:27017/todos'
ENV APP_PORT='3002'
WORKDIR  /demo/back-end
COPY . /demo/back-end
RUN npm ci
RUN npm run lint
CMD [ "npm", "run", "dev" ]
CMD [ "npm", "run", "start" ]
EXPOSE 3002
