FROM node:alpine AS build
WORKDIR /usr/src/app
COPY package.json ./
RUN npm install --legacy-peer-deps
COPY . .
RUN npm run build
RUN npm install serve -g

CMD ["serve", "-s", "dist/browser", "-l", "4200"]