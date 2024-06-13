# docker learnings
Aims:
- Learn how to deploy a project in docker
- Understand how docker works

Check your images:
docker images

Pull a new image:
docker pull {image_name}:{version}

Check containers:
docker ps
-a list all containers

Run your image:
docker run {tag} {image_name}
--name assign a name to the container
-d run container in background
-p {exposed_port_number:port_number} publish a container's port to the host
Example
sudo docker run --name web-app -d -p 9000:80 nginx

Build private docker image
docker build {tag} 
-t {app_name:version} sets a name eg -t node-app:1.0

Check container log
docker logs {image_name}

Start a container
docker start {container_name}

Stop a container
docker stop {container}

Port binding
Keep the exposed local host number the same as conatner port number
