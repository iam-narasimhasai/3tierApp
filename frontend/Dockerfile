FROM node:14

WORKDIR /app

COPY package*.json .

RUN npm install

COPY . .

ENV REACT_APP_API_URL http://localhost:321/goals

EXPOSE 3000

CMD ["npm","start"]