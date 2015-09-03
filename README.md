# sample-app-httpd
Repository to build docker container image of sample application http server 

# Build Docker image by [Packer](http://www.packer.io/)

## How to run

Install Docker and Packer and execute the following commands

```
$ packer validate sample-app-httpd.json
$ packer build -var 'version=v1.0.0' sample-app-httpd.json
```
Once packer creates the container, ansible provisions the container. Once container is provisioned, an image is created and pushed to docker index.
