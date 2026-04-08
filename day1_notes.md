# Day1 - Docker Intro: Images, Containers, Basic Commands

## Theory
- A container is a lightweight, isolated environment to run your application
- Same app, same behaviour, everywhere — your laptop, staging, production
- No more "it works on my machine"

## Key Concepts
- **Image** = Blueprint/template. Read-only. Like a class in programming.
- **Container** = Running instance of an image. Like an object from a class.
- **Dockerfile** = Instructions to build an image.
- **DockerHub** = Public registry of images. Like GitHub but for Docker images.
- **docker-compose** = Tool to run multiple containers together.

## Commands Learned

| Command | What it does |
|---------|-------------|
| `docker --version` | Check Docker is installed |
| `docker pull ubuntu` | Download ubuntu image from DockerHub |
| `docker images` | List all images on your machine |
| `docker run ubuntu echo hi` | Run container, execute command, stop |
| `docker run -it ubuntu bash` | Run container interactively (get a shell!) |
| `docker ps` | List RUNNING containers |
| `docker ps -a` | List ALL containers including stopped |
| `docker stop CONTAINER_ID` | Stop a running container |
| `docker start CONTAINER_ID` | Start a stopped container |
| `docker rm CONTAINER_ID` | Delete a container |
| `docker rmi IMAGE_ID` | Delete an image |
| `docker run -d nginx` | Run nginx in background (detached) |
| `docker run -d -p 8080:80 nginx` | Map port 8080 on host to port 80 in container |
| `docker logs CONTAINER_ID` | See container logs |
| `docker exec -it ID bash` | Enter a running container shell |
| `docker inspect CONTAINER_ID` | Detailed info about container |
| `docker stats` | Live resource usage of all containers |

## Key Takeaways
- `docker run -it` = interactive terminal — you get a shell inside the container
- `-d` = detached mode — runs in background, you get your terminal back
- `-p 8080:80` = port mapping — host:container
- `docker ps -a` shows ALL containers — running and stopped
- `docker exec -it ID bash` = enter a running container without stopping it
- Every `docker run` creates a NEW container — old ones pile up, use `docker rm`
- `docker stats` = live CPU/memory usage — like `top` but for containers>
```

