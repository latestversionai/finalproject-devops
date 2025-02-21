# Containerization
> This is a reference for using docker in a CLI environment. (Red Hat Linux 9 was the referenced operating system)

* *sudo* sudo [ dnf/apt ] config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo | download the Docker repository.

* *sudo* [ dnf/apt ] install -y docker-ce docker-ce-cli containerd.io docker-compose-plugin | install the dependencies of Docker. 

* *sudo* systemctl start docker     | start docker in your Red Hat Instance
* *sudo* systemctl enable docker    | Enable Docker in your instance (it will start at startup)

## Syntax of Docker

* *docker* pull **imagename**:latest        | This will pull an -image- from Dockerhub
* *docker* run **imagename**                | Run a container, replicate of the image pulled.

* *docker* ps                               | Show the docker *processes* running; add option -a for all
* *docker* stop ..x..x..                    | define the image to stop (either by given name or process ID)

### "Options" of docker