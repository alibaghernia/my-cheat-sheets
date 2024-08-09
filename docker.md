`docker logs -f <container-id-or-name>`

`docker rm -f <container-id>`

`docker rmi <img-name>`

`docker rmi <img-name>`

`docker ps`


```bash
docker run 
-p <local-port>:<container-port> #8080:80
-e <var-name>=<var-value>
--network <network-name>
<image-name>:<tag>
```



# Volume
`docekr volume create <volume-name>`

`docekr volume ls`

`docekr volume inspect <volume-name>`

`docekr volume remove <volume-name>`

# Network
`docker network create <network-name>`

`docker network ls`



