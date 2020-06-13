FROM node
WORKDIR  /usr/app
COPY . /usr/app
ENV MONGO_URI='mongodb://mongo:27017/todos'
ENV APP_PORT='3002'
RUN npm ci
RUN npm run lint
EXPOSE 3002
CMD [ "npm", "run", "dev" ]
CMD [ "npm", "run", "start" ]
