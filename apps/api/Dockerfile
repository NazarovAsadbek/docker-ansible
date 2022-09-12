FROM node:14-alpine
WORKDIR /opt/app
ADD *.json .
RUN npm install
ADD . .
RUN npm run build api
CMD ["node", "./dist/apps/api/main.js"]