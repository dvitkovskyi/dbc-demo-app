
FROM node:12.16.1 
ENV MONGO_URI='mongodb://mongo:27017/todos'
ENV APP_PORT='3002'
WORKDIR  /opt/back-end
COPY . /opt/back-end
RUN npm ci
RUN npm run lint
CMD [ "npm", "run", "dev" ]
CMD [ "npm", "run", "start" ]
EXPOSE 3002
