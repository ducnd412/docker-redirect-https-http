# HTTPs to HTTP redirect

[![hope/redirect-http-to-https](https://img.shields.io/badge/docker-hope/redirect--http--to--https-brightgreen.svg)](https://hub.docker.com/r/ducnd412/redirect-https-to-http/)

Small container, that simply redirects all HTTPS requests to HTTP.
Can be used with rancher Load balancer.  
Based on Nginx and Alpine.  

## Run

Build image

    docker build -t redirect .
      
Run container

    docker run -d -p 80:80 --name=redirect redirect
