FROM node:11.9.0-alpine

ENV PORT=8080
EXPOSE 8080

WORKDIR /app

COPY package*.json ./
RUN npm install --only=production
COPY dist dist 
CMD ["yarn", "start"]