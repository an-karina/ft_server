# ft_server

You mast run docker-machine, create image, container and after that you can build and run docker.

if (machine doesnt exist)

  docker-machine create default
  
else

{
    docker-machine stop default
    
    docker-machine rm default
    
    docker-machine create default
    
}

eval $(docker-machine env)

docker build PATH

docker run -p 80:80 -p 443:443 -d <image>
  
docker exec -it <container> bash
