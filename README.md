# Docker Compose Repository

This repository contains Docker Compose configurations. Each service has its own folder with a `docker-compose.yml` file.

## How to Run

To run the Docker Compose configuration, follow these steps:

1. Navigate to the folder of the desired service.
    ```bash
    cd service-folder
    ```

2. Run the following command to start the services:
    ```bash
    docker-compose up
    ```
    - This command will create and start the services as defined in the `docker-compose.yml` file.
  
    Optionally, if you want to run the services in the background, you can use the following command:
    ```bash
    docker-compose up -d
    ```
   - The `-d` flag stands for "detached" mode, which runs the services in the background.

## How to Stop

To stop the running services, use the following command:
```bash
docker-compose down
```
## Additional Commands

### Inspect Containers

To inspect the running containers, you can use the following command:
```bash
docker-compose ps
```

###  Check Network Details
To check the details of the network created by Docker Compose, use the following command:
```bash
docker-compose network ls
```

###  View Logs
To view the logs of the running containers, you can use the following command:
```bash
docker-compose logs
```

###  Build Services
If changes are made to the services or Dockerfiles, you can use the following command to rebuild the services:
```bash
docker-compose build
```

###  Remove Containers, Networks, and Volumes
To remove stopped containers, networks, and volumes defined in the `docker-compose.yml` file, you can use the following command:
```bash
docker-compose down -v
```
 - The `-v` flag removes volumes associated with the services.

Feel free to explore other Docker and Docker Compose commands for additional functionalities. You can refer to the official Docker documentation for more details: [Docker Documentation](https://docs.docker.com/)
