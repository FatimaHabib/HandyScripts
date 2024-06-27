## Docker:
Docker is  a platform or an ecosystem around creating and running containairs. It makes really easy to install and run software without worrying about setup or dependencies.
## Container:
It is a process or a group of processes that has resources specifically assaigned to it. Each container is an instance of an Image.
## Image:
Is a single file with all the dependencies and configurations required to run a program. Each image composes of two components:
 <ol>
  <li>File system snapshot.</li>
  <li>Start up command (deafault command): it is excuted when a container of the image is running. </li>
  
  </ol>
  
  ## Docker characteristics:
   <ul>
<li> Name spacing:  isolating resources per process or group of processes.</li>
<li>Control groups: limit amout o fresources used per process.</li>
</ul>

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

