### Packer project to produce Vagrant Image with Docker and Docker Compose

This project creates a Vagrant VirtualBox image consisting of Docker 1.12.3 and Docker Compose 1.8.0 versions

Steps to use the VirtualBox Vagrant image:

1. Build the image using Packer.

  ```shell
  $ packer build docker-ubuntu1604.json
  ```

2. Run the Vagrant VirtualBox image.

  ```shell
  $ vagrant up virtualbox
  ```
  
3. SSH into the image and use it.

  ```shell
  $ vagrant ssh virtualbox
  ```
