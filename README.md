# Learning How to use Docker

# Installing Docker in Linux using command 

`apt install docker.io`

# Checking status of Docker

After Installation check if you getting any output using command `docker --version`

To check if your docker is active or not run command `sudo systemctl status docker` check the Active value .

To set Active value to Active: active run the command `sudo systemctl enable --now docker`

# Pushing Your App to Docker repository 

Firest we need to add commands in our Dockerfile and then build our docker image 

Command to build our docker image  `docker build -t codestormer/hello-codestormer-docker .` we use . because we were in the same directory in which we had our Dockerfile

Create a docker repository and then run  `docker push codestormer/hello-codestormer-docker:hello-codestormer-docker`

`codestormer` is the username 

`hello-codestormer-docker` is the name of the repository



# Pulling A Docker File
`docker pull codestormer/hello-codestormer-docker`

# Checking your images
`docker image ls`

# Running your docker image
`docker run `codestormer/hello-codestormer-docker`
