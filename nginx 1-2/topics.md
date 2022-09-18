The Nginx Mastery Series.

Introducing Nginx

- [x] Getting started with Docker and Nginx
    - [x] Pull image from Docker --> docker pull {image name}
    - [x] Run Nginx container --> docker run {image name} (in general) and if specifically docker run -it --rm -d -p 8080:80 --name {name what your container}
    - [x] Docker stop container --> docker rm {container id/name} -f (for running container)
    - [x] Verifying your installation
        - [x] nginx -v
        - [x] Docker top web --> docker top {container name} and similar function which can be used inside shell {ps -C nginx -f}
        - [x] curl localhost --> write command curl localhost:8000 it will give you what html page will show you for nginx
        - [x] Browser localhost:8080
    - [x] Basic Service management
        - [x] service nginx start
        - [x] service nginx stop
        - [x] Nginx commands  --> (nginx -h, nginx -s reload, nginx -t)
            - [x] -h (help command)
            - [x] -v -V
            - [x] -t -T
            - [x] -s signal  --> (signal example stop, start, reload)
    - [x] Nginx default folder /usr/share/nginx/html
    - [x] Docker-compose file - using volumes
    - [x] Serving custom pages - index.html
    - [x] Building a new Nginx image --> (docker build -t {image name} .)
        - [x] DockerFile
