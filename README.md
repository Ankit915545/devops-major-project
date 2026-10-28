# DevOps Major Project

## Project Overview
   This project demonstrates how to package and serve a static HTML website using Docker and Nginx.
   Version V4 contains the updated project title, version information, author name, and an explanation 
   of Docker and Nginx.

## Dockerfile explanation
   The Dockerfile defines how the application image is built. It uses an Nginx base image and copies the website's HTML    file into Nginx's web root directory so the page can be served over HTTP.

## Image build command
   
   docker build -t devops-major-project:v4 .

## Container run command
   
   docker run -d --name devops-web-v4-test -p 8087:80 devops-major-project:v4

## Application Verification commands

  ## Check the HTTP response:

      curl -I http://localhost:8087

  ## Display the HTML page:

      curl http://localhost:8087

  ## Check the running container:

      docker ps

## Troubleshooting Commands
 
   docker logs devops-web-v4-test
   docker inspect devops-web-v4-test
   docker port devops-web-v4-test





