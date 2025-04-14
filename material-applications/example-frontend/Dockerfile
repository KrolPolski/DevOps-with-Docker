
FROM node:16

EXPOSE 5000

ENV REACT_APP_BACKEND_URL=http://127.0.0.1:8080/
WORKDIR /usr/src/app

COPY . .

RUN npm install -g serve

RUN npm install react-scripts

RUN npm run build

CMD ["serve", "-s", "-l", "5000", "build"]