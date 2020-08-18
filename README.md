# How to install docker and deploy postgres docker image using LinuxONE Community Cloud
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


### Step 3:Running Postgres docker images
  3.1 Run postgres docker image as a container 
   ```sh
   # docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres
   ```
   ![alt text](images/docker_run.png "Check /data disk")

  3.2 After succesfully running last command, you can now check the running container 
   ```sh
   # docker ps
   ```
   ![alt text](images/docker_ps.png "Check /data disk")
   
   3.3 Now you can execture Postgres container 
   ```sh
   # docker exec -it some-postgres bash
   ```
   ![alt text](images/docker_exec.png "Check /data disk")
   
  3.4 connect to postgresql using user postgres 
   ```sh
   # psql -U postgres
   ```
   ![alt text](images/docker_postgres.png "Check /data disk")
