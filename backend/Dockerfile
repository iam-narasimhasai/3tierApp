FROM node:23-alpine

WORKDIR /app

COPY package*.json .

RUN npm ci --only=production

COPY . .

EXPOSE 3000 

ENV MONGO_URL=mongodb://localhost:27017/course-goals

ENV PORT=3000

CMD ["node","app.js"]
