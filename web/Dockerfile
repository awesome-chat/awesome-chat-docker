FROM node:9.4.0

WORKDIR /src

# is git available?
RUN git clone https://github.com/wengwengweng/awesome-chat-web.git

WORKDIR /src/awesome-chat-web

RUN npm install --registry=https://registry.npm.taobao.org

RUN npm run build

RUN npm install pm2 -g --registry=https://registry.npm.taobao.org

EXPOSE 3000

# run pm2
CMD ["npm", "start"]