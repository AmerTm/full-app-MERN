FROM node:12.2.0-alpine

WORKDIR /client

ENV PATH /app/node_modules/.bin:$PATH

COPY package*.json ./
RUN npm install
RUN npm install react-scripts@3.0.1 -g

COPY . .
EXPOSE 3000
CMD ["npm", "start"]