# TeaStore_SingleContainer

`http://localhost:8080/tools.descartes.teastore.webui/`


`sudo docker build -f Dockerfile -t roshin-ust/teastore .`

`docker run -p 3306:3306 -d --name teastore-db descartesresearch/teastore-db`


`docker run -p 8080:8080 -d --link teastore-db:teastore-db --name teastore-roshin roshin-ust/teastore`

`sudo docker container stop teastore-roshin`
`sudo docker container rm teastore-roshin`
`sudo docker images`
`sudo docker rmi roshin-ust/teastore`
