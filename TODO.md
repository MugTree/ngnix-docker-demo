# Ngnix reverse proxy with a series of containerised apps behind it

https://www.digitalocean.com/community/tutorials/how-to-configure-nginx-as-a-reverse-proxy-on-ubuntu-22-04

## Outline

- Docker create a two stage build
- Build stage and runtime stage for a simpler smaller final image

## Basic procedure per app

1. Build
2. Push the image to a registry
3. Shh into the vps
4. Login to the registry
5. Pull the image
6. Stop and remove the old container
7. run new container with the updated image
