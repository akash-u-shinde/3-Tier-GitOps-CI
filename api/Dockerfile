FROM node:20-alpine

WORKDIR /app
COPY package*.json ./
RUN npm cache clean --force
RUN npm ci --prefer-offline --no-audit
COPY . .
EXPOSE 5000
CMD ["node", "app.js"]

