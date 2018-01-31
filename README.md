# Homework 14

Q: Why the outputs of these two commands

```
docker inspect <u_container_id>
```

```
docker inspect <u_image_id>
```

differ?

A: The first command outputs low-level metadata, describing docker container, while the second one outputs metadata describing docker image. These are two different docker entities. docker container is an instance of docker image and its metadata contains such concrete information as network configuration etc. And as of docker image, its metadata contains information about lower layers on top of which this image is built. So, these are two different entities, which serve different purposes.
