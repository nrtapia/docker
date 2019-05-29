# Docker TIPS #


### Ejecutar terminal en un contenedor ###
- docker exec -it [container] bash

### Ejecutar la terminal de la VM de Docker en MAC ###

- docker run -it --rm --privileged --pid=host justincormack/nsenter1 

https://gist.github.com/BretFisher/5e1a0c7bcca4c735e716abf62afad389


### Construir una imagen desde un Dockerfile ###
- docker build --build-arg [ARGUMENT_NAME]=[argument_value] . -t [IMAGE_NAME]:[IMAGE_VERSION]  --no-cache

### Construir un conteneder desde una imagen ###
- docker run --name [CONTAINER_NAME] -p 80:80 [IMAGE_NAME]:[IMAGE_VERSION]
