FROM node:9.4.0

RUN mkdir -p /usr/src/aweasome-chat

COPY ./awesome-chat-web /usr/src/aweasome-chat

WORKDIR /usr/src/aweasome-chat

RUN npm install --registry=https://registry.npm.taobao.org

RUN npm run dev

EXPOSE 3000

# run pm2
CMD ["npm", "start"]