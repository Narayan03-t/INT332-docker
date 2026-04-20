# Docker Commands Used

## Pull Image

```bash
docker pull mysql
```

## Run Container

```bash
docker run -it --name my-db -e MYSQL_ROOT_PASSWORD=**** mysql:latest
```

## Check Running Containers

```bash
docker ps
```

## Access Container

```bash
docker exec -it my-db bash
```
