# Day 19 Task: Docker for DevOps Engineers
Till now you have learn how to create docker-compose.yml file and pushed it to the Repository. Let's move forward and dig more on other Docker-compose.yml concepts. Aj thodi padhai krte hai on Docker Volume & Docker Network 😃

## Task-01

- Create a multi-container application using docker-compose and mount a volume on multiple services. ( Hint - Create application and database container )
- Use the `docker-compose up` command with the `-d` flag to start a multi-container application in detached mode.
- Use the `docker-compose scale` command to increase or decrease the number of replicas for a specific service.
- Use the `docker-compose ps` command to view the status of all containers, and `docker-compose logs` to view the logs of a specific service.
- Use the `docker-compose down` command to stop and remove all containers, networks, and volumes associated with the application

- Learn how to use Docker Volumes and Named Volumes to share files and directories between multiple containers.
- Create two or more containers that read and write data to the same volume using the `docker run --mount` command.
- Verify that the data is the same in all containers by using the docker exec command to run commands inside each container.
- Use the docker volume ls command to list all volumes and docker volume rm command to remove the volume when you're done.

