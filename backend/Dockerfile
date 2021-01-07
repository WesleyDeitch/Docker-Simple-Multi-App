FROM node

WORKDIR /app

COPY ./package.json /app

RUN npm install

COPY . .

EXPOSE 80

VOLUME [ "/app/node_modules" ]

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret

CMD ["npm", "start"]