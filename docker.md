### Starting a Docker server
```
sudo service docker start
```


### Creating and running container from an image:

```
docker run <Image name>
```
### Overriding default command: 
the new command will be excuted instead of the default command.
```
docker run <Image name> new command 
```

### Listing running containers:

```
docker ps
```
### Listing all the running containers that we have ever created 

```
docker ps --all
```
### Creating a container (no running):
```
docker creat <Image name>
```
### Running the created container:
-a: gives the output of the running process.
```
docker start -a container_ID
```
### Removestoped containers:
```
docker system prune
```
### Retriving log outputs:

-Instead of rerun a container which could be quitly expensive.
```
docker logs <container_ID>
```
### Delete an image 
docker rmi <image_id>

