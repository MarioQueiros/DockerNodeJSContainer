#DockerNodeJSContainer

A NodeJS Docker container

`docker build -t marioqueiros/node .`

`docker run -v ~/node2/src/:/mnt -d --name node -p 8080 marioqueiros/node`

The command mounts a host dir on the container

`-v ~/node2/src/:/mnt`

###Command to execute bash inside container

`sudo docker exec -i -t node bash`

### Update files inside container
Copy files from mnt folder to the app source folder

`cp -avr /mnt /src/src`