# postgres-on-docker
Running postgresql on docker

## Prerequisites
 1. Request access to LinuxONE Community Cloud. Follow instructions [here](https://github.com/Elvin94/LinuxONE-OSS-CC)


  ### Step 1: Install docker
   
   1.1 install docker
   ```sh
   # sudo yum install docker 
   ```
  1.2 Ensure docker installed by checking version
   ```sh
   # sudo docker version
   ```
   ![alt text](images/docker_version.png "Check /data disk")
   
  ### Step 2: Download Postgres image
  2.1 Pull postgres docker image  
   ```sh
   # sudo docker pull postgres:latest
   ```
   ![alt text](images/docker-pull-postgres.png "Check /data disk")

  2.2 List docker images 
   ```sh
   # sudo docker images
   ```
   ![alt text](images/docker_images.png "Check /data disk")
