# Steps

- Clone repo  
  `git clone https://github.com/mrckurz/cd2020-ex04`
- Create docker image  
  `docker image build -f Dockerfile -t andreasroither/my-first-image:0.0.1 ./`
- Push image to docker hub  
  `docker image push andreasroither/my-first-image:0.0.1`
- Create a new image:  
  `docker image build -t andreasroither/myhello:0.0.1 ./`
- Run container on port 9090
  `docker container run -p 9090:8888 --name myhello andreasroither/myhello:0.0.1`
- Stop the container
  `docker stop myhello` 

# Useful docker commands
- `docker login`
- `docker images`
- `docker ps -a` 