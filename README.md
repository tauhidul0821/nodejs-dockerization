```shell
FROM node:9-slim
WORKDIR /app
COPY package.json /app
RUN npm install
COPY . /app
CMD ["npm","start"]
```

docker build -t node-docker-tutorial .
docker build -t node-docker-tutorial .
docker ps
docker images
docker run -it -p 4600:3000 -v $(pwd):/app node-docker-tutorial