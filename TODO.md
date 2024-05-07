## Outline per app

- Assumes we are using a hosted database
- Docker... Create a two stage build stage and runtime stage for a simpler smaller final image

## Basic procedure per app

Likely automated with a shell script or a build process using github actions or somesuch..

1. Build image
2. Push the image to a registry
3. SHH into the VPS
4. Login to the Registry
5. Pull the image from the Registry
6. Stop and remove the old container
7. Run new container with the updated image

# Notes

#### Ngnix reverse proxy with a series of containerised apps behind it

https://www.digitalocean.com/community/tutorials/how-to-configure-nginx-as-a-reverse-proxy-on-ubuntu-22-04
