# Online Spy

![Build status](https://img.shields.io/github/workflow/status/VeryBadFrags/online-spy/NodeCI)
![License: MIT](https://img.shields.io/badge/license-MIT-green)

A multiplayer social deduction game inspired by [Spyfall](https://hwint.ru/portfolio-item/spyfall/). Built with Node and [socket.io](https://socket.io).

[▶️ Play the game](https://spy.verybadfrags.com)

## Run with Node

Install the Node nodules and start the server

```sh
npm i
npm start
```


## Develop locally

```sh
npm i
npm run dev
```

## Docker

Run locally

```sh
docker-compose up
```

Push image to Docker Hub

```sh
docker-compose build
docker image tag online-spy_web verybadfrags/online-spy
docker push verybadfrags/online-spy
```

Deploy on remote server

```sh
docker stop online-spy
docker rm online-spy
docker run -d --restart unless-stopped --pull always -p 8081:8081 --name online-spy verybadfrags/online-spy
```
