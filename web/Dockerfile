FROM node:9.4.0

COPY /home/weng/aweasome-chat/awesome-chat-web /usr/src/aweasome-chat

WORKDIR /usr/src/aweasome-chat

RUN npm install --registry=https://registry.npm.taobao.org

RUN npm run build

RUN npm install pm2 -g --registry=https://registry.npm.taobao.org

EXPOSE 3000

# run pm2
CMD ["npm", "start"]