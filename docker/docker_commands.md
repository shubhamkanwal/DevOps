#Docker commands
 Basic
 
1. To run docker image 
   docker run <docker-image>
2. To view all images
   docker images -a
3. To view all containers
   docker ps -a
4. To view all running containers
   docker ps 
5. To stop running containers
   -One by one-
    docker stop <container id> <container id> <container id> .....
   -All at once-
    docker stop $(docker ps -aq)
6. To delete stopped containers
   -One by one-
   docker rm <container id>
   -All at once-
   docker rm $(docker ps -aq)
7. To delete a image
   -One by one-
   docker rmi <image-name>
   -All at once-
   docker rmi $(docker images -aq)
8. To pull a docker image and do not create a container for it
   docker pull <image-name>
9. To run a container in detach mode(background) with a particular image and name the container
   docker run -d --name <your-container> <image-name>



