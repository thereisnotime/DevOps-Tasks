# DevOps-Tasks

Basic DevOps hands-on tasks for beginners looking to learn the ropes. This is a work in progress and will be updated as we go along.

Table of Contents:

- [DevOps-Tasks](#devops-tasks)
  - [Pre-requisites](#pre-requisites)
    - [Learning](#learning)
    - [Tools](#tools)
    - [Services](#services)
    - [Extra](#extra)
  - [Task 1: Starting apps](#task-1-starting-apps)
    - [Task 1.1 Docker](#task-11-docker)
      - [Task 1.1.1 Postgre Server and Client](#task-111-postgre-server-and-client)
      - [Task 1.1.2 MySQL Server and Client](#task-112-mysql-server-and-client)
      - [Task 1.1.3 MongoDB Server and Client](#task-113-mongodb-server-and-client)
      - [Task 1.1.4 Redis Server and Client](#task-114-redis-server-and-client)
      - [Task 1.1.5 Your Website](#task-115-your-website)
      - [Task 1.1.5 Your Docker Image](#task-115-your-docker-image)
      - [Task 1.1.6 Docker Exec](#task-116-docker-exec)
      - [Task 1.1.7 Docker Environment Variables](#task-117-docker-environment-variables)
      - [Task 1.1.8 Docker Volumes](#task-118-docker-volumes)
      - [Task 1.1.9 Docker Networks](#task-119-docker-networks)
      - [Task 1.1.10 Docker Commit](#task-1110-docker-commit)
      - [Task 1.1.11 Dockerfile and Justauser](#task-1111-dockerfile-and-justauser)
    - [Task 1.2 Docker-compose](#task-12-docker-compose)
      - [Task 1.2.1 Docker Compose Up/Down/Start/Stop](#task-121-docker-compose-updownstartstop)
      - [Task 1.2.2 Docker Compose Logs](#task-122-docker-compose-logs)
      - [Task 1.2.3 Docker Compose Ps](#task-123-docker-compose-ps)
      - [Task 1.2.4 Docker Compose Exec](#task-124-docker-compose-exec)
      - [Task 1.2.5 Docker Compose Scale](#task-125-docker-compose-scale)
      - [Task 1.2.6 Docker Compose Top](#task-126-docker-compose-top)
      - [Task 1.2.7 Running a Single Service](#task-127-running-a-single-service)
      - [Task 1.2.8 Running Multiple Services](#task-128-running-multiple-services)
      - [Task 1.2.9 Your Compose](#task-129-your-compose)
      - [Task 1.2.10 Your Compose from Source](#task-1210-your-compose-from-source)
    - [Task 1.3 Kubernetes](#task-13-kubernetes)
      - [Task 1.3.1 Starting a Cluster](#task-131-starting-a-cluster)
      - [Task 1.3.2 Connecting to the Cluster](#task-132-connecting-to-the-cluster)
      - [Task 1.3.3 Creating a Pod](#task-133-creating-a-pod)
      - [Task 1.3.4 Creating a Deployment](#task-134-creating-a-deployment)
      - [Task 1.3.5 Creating a StatefulSet](#task-135-creating-a-statefulset)
      - [Task 1.3.6 Creating a Secret](#task-136-creating-a-secret)
      - [Task 1.3.7 Creating a ConfigMap](#task-137-creating-a-configmap)
      - [Task 1.3.8 Creating a Service](#task-138-creating-a-service)
      - [Task 1.3.9 Creating an Ingress](#task-139-creating-an-ingress)
      - [Task 1.3.10 Performing a Rollout Restart](#task-1310-performing-a-rollout-restart)
      - [Task 1.3.11 Patching a Resource](#task-1311-patching-a-resource)
      - [Task 1.3.12 Creating a Persistent Volume and Persistent Volume Claim](#task-1312-creating-a-persistent-volume-and-persistent-volume-claim)
      - [Task 1.3.13 Updating a Deployment to Use a Persistent Volume](#task-1313-updating-a-deployment-to-use-a-persistent-volume)
      - [Task 1.3.14 Creating a Horizontal Pod Autoscaler](#task-1314-creating-a-horizontal-pod-autoscaler)
      - [Task 1.3.15 Creating a Network Policy](#task-1315-creating-a-network-policy)
      - [Task 1.3.16 Creating a Job](#task-1316-creating-a-job)
  - [Task 2: Pipelines](#task-2-pipelines)
    - [Task 2.1 Jenkins](#task-21-jenkins)
    - [Task 2.2 Gitlab](#task-22-gitlab)
    - [Task 2.3 Github](#task-23-github)
  - [Task 3: Data Formats](#task-3-data-formats)
    - [Task 3.1 JSON](#task-31-json)
    - [Task 3.2 YAML](#task-32-yaml)
    - [Task 3.3 TOML](#task-33-toml)
    - [Task 3.4 XML](#task-34-xml)
    - [Task 3.5 CSV](#task-35-csv)
    - [Task 3.6 INI](#task-36-ini)
  - [Task 4: Infrastructure as Code](#task-4-infrastructure-as-code)
    - [Task 4.1 Terraform](#task-41-terraform)
    - [Task 4.2 Ansible](#task-42-ansible)
    - [Task 4.3 Pulumi](#task-43-pulumi)
    - [Task 4.4 Puppet](#task-44-puppet)
    - [Task 4.5 Chef](#task-45-chef)
    - [Task 4.6 SaltStack](#task-46-saltstack)
  - [Task 5: Cloud Providers](#task-5-cloud-providers)
    - [Task 5.1 AWS](#task-51-aws)
    - [Task 5.2 Azure](#task-52-azure)
    - [Task 5.3 GCP](#task-53-gcp)
    - [Task 5.4 Oracle](#task-54-oracle)
    - [Task 5.5 Digital Ocean](#task-55-digital-ocean)
    - [Task 5.6 Linode](#task-56-linode)
  - [Questions](#questions)
  - [Terms, buzzwords and more](#terms-buzzwords-and-more)

## Pre-requisites

### Learning

Few important notes on how to research and learn:

- [Google](https://www.google.com) is your best friend. You can find anything you want, including the official documentation.
- [Stackoverflow](https://stackoverflow.com) is your second best friend. There is always someone who had the same problem as you.
- [Youtube](https://www.youtube.com) is your third best friend. There is always a video explaining what you are looking for.
- [Reddit](https://www.reddit.com) is your fourth best friend. There is always a community that can help you.

Also most of the tools have communities in Reddit, Discord, Slack, Glip etc. It is good to join them and ask questions if you are stuck.

A good professional is always up-to date with the latest news and trends. For starters you can use the following websites and channels to keep up:

- [PowerCert](https://www.youtube.com/channel/UCJQJ4GjTiq5lmn8czf8oo0Q)
- [A Cloud Guru](https://www.youtube.com/channel/UCp8lLM2JP_1pv6E0NQ38pqw)
- [TLF](https://www.youtube.com/channel/UCfX55Sx5hEFjoC3cNs6mCUQ)
- [Coding Tech](https://www.youtube.com/channel/UCtxCXg-UvSnTKPOzLH4wJaQ)
- [Crosstalk Solutions](https://www.youtube.com/channel/UCVS6ejD9NLZvjsvhcbiDzjw)
- [ExplainingComputers](https://www.youtube.com/channel/UCbiGcwDWZjz05njNPrJU7jA)
- [Linux For Everyone](https://www.youtube.com/channel/UCd4XwUn2Lure2NHHjukoCwA)
- [The Linux Experiment](https://www.youtube.com/channel/UC5UAwBUum7CPN5buc-_N1Fw)
- [DistroTube](https://www.youtube.com/channel/UCVls1GmFKf6WlTraIb_IaJg)
- [Craft Computing](https://www.youtube.com/channel/UCp3yVOm6A55nx65STpm3tXQ)
- [Gary Explains](https://www.youtube.com/channel/UCRjSO-juFtngAeJGJRMdIZw)
- [Simplilearn](https://www.youtube.com/channel/UCsvqVGtbbyHaMoevxPAq9Fg)
- [CBT Nuggets](https://www.youtube.com/channel/UClIFqsmxnwVNNlsvjH1D1Aw)
- [NCIX Tech Tips](https://www.youtube.com/channel/UCjTCFFq605uuq4YN4VmhkBA)
- [Just me and Open Source](https://www.youtube.com/channel/UC6VkhPuCCwR_kG0GExjoozg)
- [NixieDoesLinux](https://www.youtube.com/channel/UCBE-FO9JUOghSysV9gjTeHw)
- [Amit Nepal](https://www.youtube.com/channel/UCIOlfUXD5wYP_uEemv2_LVg)
- [SysAdminGirl](https://www.youtube.com/channel/UCkIHLaOEtdLpC3JrqR3Bwmw)
- [Coding Tech](https://www.youtube.com/channel/UCtxCXg-UvSnTKPOzLH4wJaQ)
- [Computerphile](https://www.youtube.com/channel/UC9-y-6csu5WGm29I7JiwpnA)
- [GotoConferences](https://www.youtube.com/c/GotoConferences)
- [elithecomputerguy](https://www.youtube.com/user/elithecomputerguy)
- [NetworkChuck](https://www.youtube.com/c/NetworkChuck)
- [TechWorldwithNana](https://www.youtube.com/c/TechWorldwithNana)

When you are not sure about what is out there in terms of technologies and resources, always consult with your local awesome list:

- [AcalephStorage/awesome-devops](https://github.com/AcalephStorage/awesome-devops)
- [awesome-soft/awesome-devops](https://github.com/awesome-soft/awesome-devops)
- [Lets-DevOps/awesome-learning](https://github.com/Lets-DevOps/awesome-learning)
- [AcalephStorage/awesome-devops](https://github.com/AcalephStorage/awesome-devops)
- [awesome-selfhosted/awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted)
- [juandecarrion/awesome-self-hosted](https://github.com/juandecarrion/awesome-self-hosted)
- [kahun/awesome-sysadmin](https://github.com/kahun/awesome-sysadmin)
- [epcim/awesome-sysadmin2](https://github.com/epcim/awesome-sysadmin2)
- [devops-roadma](https://github.com/raycad/devops-roadmap)

### Tools

In order to move forward, it is better to have a virtual machine running Ubuntu 22.04 (or latest stable) with the following tools (latest stable versions) installed:

- asdf
- git
- docker
- minikube
- terraform (via asdf)
- kubectl (via asdf)
- helm (via asdf)
- nodejs (via asdf)
- npm (via asdf)
- ansible (via asdf)
- jq
- curl
- wget
- DBeaver
- MongoDB Compass
- Redis Commander

You can find the official documentations to see how to install and configure the tools.

### Services

To ease your way into the DevOps world, we will be using the following services:

- Register at [GitHub.com](https://github.com).
- Register at [GitLab.com](https://gitlab.com).
- Register at [Azure DevOps](https://azure.microsoft.com/en-us/pricing/details/devops/azure-devops-services/).
- Register at [Docker Hub](https://hub.docker.com).
- Register at [Oracle](https://youtu.be/NKc3k7xceT8) for a free VM.
- Register at [Cloudflare](https://www.cloudflare.com/) for managing DNS zones.
-

### Extra

- If you are a student (or have a student email), get the [GitHub Student Developer Pack](https://education.github.com/pack).

## Task 1: Starting apps

TODO

### Task 1.1 Docker

TODO

#### Task 1.1.1 Postgre Server and Client

Start the latest stable Postgre server via docker run command. The server should be accessible from the host machine. In another container run psql (Postgre client CLI) and connect to the server.

DoD:

- You must be able to view the Postgre server version from the client via command, be able to CRUD databases and get the size of all databases.

Bonus: Also do it via GUI (ex. DBeaver).

#### Task 1.1.2 MySQL Server and Client

Start the latest stable MySQL server via docker run command. The server should be accessible from the host machine. In another container run mysql (MySQL client CLI) and connect to the server.

DoD:

- You must be able to view the MySQL server version from the client via command, be able to CRUD databases and get the size of all databases.

Bonus: Also do it via GUI (ex. DBeaver).

#### Task 1.1.3 MongoDB Server and Client

Start a MongoDB server with the latest version via a docker run command. The server should be accessible from the host machine. In another container, run the MongoDB client CLI (mongosh) and connect to the server.

DoD:

- You must be able to view the MongoDB server version from the client via a command, be able to CRUD collections, and retrieve the size of all collections.

Bonus: Also do it via GUI (ex. MongoDB Compass).

#### Task 1.1.4 Redis Server and Client

Start the latest stable Redis server via a docker run command. The server should be accessible from the host machine. In another container, run the Redis CLI (redis-cli) and connect to the server.

DoD:

You must be able to view the Redis server version from the client via a command, be able to CRUD data, and retrieve the size of all databases.

Bonus: Also do it via GUI (ex. Redis Commander).

#### Task 1.1.5 Your Website

Generate a simple website using ChatGPT (inline CSS, JS and HTML) and save it as index.html. In the same folder prepare Dockerfile that will use nginx:alpine as a base image and copy the index.html file to the /usr/share/nginx/html folder. Build the image and run it as a container. The website should be accessible from the host machine on port 8080.

DoD:

-You must be able to view the website from the host machine via a browser.

#### Task 1.1.5 Your Docker Image

Create a hub.docker.com account and push the image you created in the previous task to your account. The image should be public.

DoD:

- You must be able to view the image from the hub.docker.com website.

#### Task 1.1.6 Docker Exec

Run a new `alpine` container in the background. Then, use the `docker exec` command to run the `ls` command in the running container.

DoD:

- You must be able to view the output of the `ls` command from the running container.

#### Task 1.1.7 Docker Environment Variables

Create a Dockerfile that uses the `nginx:alpine` image as a base. In the Dockerfile, use the `ENV` instruction to define an environment variable `NGINX_PORT` with a default value of 8080. Then, run a container from this image, but override the `NGINX_PORT` environment variable to 8081 using the `-e` option in the `docker run` command.

DoD:

- You must be able to view the value of the `NGINX_PORT` environment variable from within the running container. You can do this by using the `docker exec` command to run the `env` command in the running container.

#### Task 1.1.8 Docker Volumes

Create a Docker volume using the `docker volume create` command. Then, run a new `nginx:alpine` container and mount the created volume to the `/usr/share/nginx/html` directory in the container. Create a simple `index.html` (write hello world inside) file in the volume (from the host machine), and verify that the file is accessible from within the container.

DoD:

- You must be able to view the `index.html` file from within the running container. You can do this by using the `docker exec` command to run the `cat` command in the running container.

Bonus: Prepare the index.html file via a shell script.

#### Task 1.1.9 Docker Networks

Create a new Docker network using the `docker network create` command. Then, run two new `alpine` containers in this network. Use the `docker exec` command to install `ping` in both containers, and then use `ping` to verify that the containers can communicate with each other over the network.

DoD:

- You must be able to successfully ping one container from the other.

#### Task 1.1.10 Docker Commit

Run a new `alpine` container, and use the `docker exec` command to install `curl` in the running container. Then, use the `docker commit` command to create a new image from the running container. Finally, run a new container from this image and verify that `curl` is installed.

DoD:

- You must be able to successfully run the `curl` command in a new container created from the committed image.

#### Task 1.1.11 Dockerfile and Justauser

Create a Dockerfile based on the latest stable Debian image. Create a file called test.txt with some sample text inside. In the Dockerfile, use the `RUN` instruction to install `curl`, `git` and `wget` in the image. Then, build the image and run a new container from it. Verify that `curl` and `wget` are installed in the running container. After that modify the Dockerfile to use a custom user called "justauser" and build the image again. Run a new container from the new image and verify that the user is "justauser". After that modify the Dockerfile to copy the test.txt file to the /home/justauser folder and build the image again. Run a new container from the new image and verify that the test.txt file is in the /home/justauser folder and justauser can read it.

DoD:

- You must be able to successfully run the `curl`, `git` and `wget` commands in a new container created from the image.
- When running `id` in the container, the user should be "justauser".
- The test.txt file should be in the /home/justauser folder and justauser should be able to read it.

### Task 1.2 Docker-compose

#### Task 1.2.1 Docker Compose Up/Down/Start/Stop

Create a Docker Compose file that defines a service to run a simple web server (for example, nginx). Use the `docker compose up` command to start the service, and verify that the web server is running correctly. Stop the service and start it again. Then, use the `docker compose down -v` command to stop the service and remove the volumes.

DoD:

- You must be able to start the service with `docker compose up` and stop it with `docker compose down -v`.
- The web server must be accessible from the host browser when the service is up.

#### Task 1.2.2 Docker Compose Logs

Start the service from the previous tasks, and then use the `docker compose logs` command to view the logs of the service.

DoD:

- You must be able to view the logs of the service with `docker compose logs`.

#### Task 1.2.3 Docker Compose Ps

Start the service from the previous tasks, and then use the `docker compose ps` command to view the status of the service.

DoD:

- You must be able to view the status of the service with `docker compose ps`.

#### Task 1.2.4 Docker Compose Exec

Start the service from the previous tasks, and then use the `docker compose exec` command to run a command (for example, `ls`) in the service container.

DoD:

- You must be able to run a command in the service container with `docker compose exec`.

#### Task 1.2.5 Docker Compose Scale

Create a Docker Compose file that defines a service to run a stateless application (for example, a web server). Use the `docker compose up --scale` command to start multiple instances of the service, and verify that all instances are running correctly.

DoD:

- You must be able to start multiple instances of the service with `docker compose up --scale`.
- All instances must be running correctly.

#### Task 1.2.6 Docker Compose Top

Start the service from the previous tasks, and then use the `docker compose top` command to view the running processes in the service container.

DoD:

- You must be able to view the running processes in the service container with `docker compose top`.

#### Task 1.2.7 Running a Single Service

Create a Docker Compose file named `docker-compose.yml` and define a service to run a single container based on <https://hub.docker.com/r/yeasy/simple-web/>. The container should expose a port, and the service should be named `myapp`. Run the service using Docker Compose.

DoD:

- The Docker Compose file `docker-compose.yml` should define a service named `myapp`.
- The service should run a single container based on an image of your choice.
- The container should expose a port.
- Running `docker-compose up` should start the service and the container.

#### Task 1.2.8 Running Multiple Services

Extend the previous Docker Compose file (`docker-compose.yml`) to define two services: `web` and `database`. The `web` service should run a container based on an image of a web application (e.g., nginx), and the `database` service should run a container based on an image of a database server (e.g., MySQL). The two services should be able to communicate with each other.

DoD:

- The Docker Compose file should define two services named `web`, `database` and `myapp`.
- The `web` service should run a container based on an image of a web application (e.g., nginx).
- You must shell into the web container, install telnet and perform a telnet to the database container on port 3306 - the connection should be successful.
- From the `web` container, you must be able to ping the database container.
- From the `web` container, you must be able to get the website running on the `myapp` container using `curl`.
- The `database` service should run a container based on an image of a database server (e.g., MySQL).
- The containers in the `web` and `database` services should be able to communicate with each other.

#### Task 1.2.9 Your Compose

Create a docker-compose.yml file that will run your website from the previous task (1.1.5). The website should be accessible from the host machine on port `9999`.

DoD:

- From the host machine, you must be able to view the website when the compose file is up via your browser.

#### Task 1.2.10 Your Compose from Source

Create a docker-compose.yml file that will build and run your image's Dockerfile from the previous task (1.1.5). The website should be accessible from the host machine on port `9999`.

DoD:

- From the host machine, you must be able to view the website when the compose file is up via your browser.

### Task 1.3 Kubernetes

#### Task 1.3.1 Starting a Cluster

Start a local Kubernetes cluster using Minikube.

DoD:

- You must be able to get the status of a local Kubernetes cluster using the `minikube status` command.
- Running `kubectl cluster-info` should display information about the running cluster.

#### Task 1.3.2 Connecting to the Cluster

Connect to the local Kubernetes cluster using `kubectl`, `k9s`, and `LENS`.

DoD:

- You must be able to view the nodes of the cluster using the `kubectl get nodes` command.
- You must be able to connect to the cluster using `k9s` and `LENS` TUI/GUI.

#### Task 1.3.3 Creating a Pod

Create a Pod named `my-pod` running the `nginx:1.14.2` image in the local Kubernetes cluster.

DoD:

- You must be able to create the Pod using `kubectl apply` with a YAML configuration file.
- Running `kubectl get pods` should display `my-pod` in the list.
- Running `kubectl describe pod my-pod` should show that the Pod is running the `nginx:1.14.2` image.

#### Task 1.3.4 Creating a Deployment

Create a Deployment named `my-deployment` running the `nginx:1.14.2` image with 3 replicas in the local Kubernetes cluster.

DoD:

- You must be able to create the Deployment using `kubectl apply` with a YAML configuration file.
- Running `kubectl get deployments` should display `my-deployment` in the list.
- Running `kubectl describe deployment my-deployment` should show that the Deployment is running 3 replicas of the `nginx:1.14.2` image.

#### Task 1.3.5 Creating a StatefulSet

Create a StatefulSet named `my-statefulset` running the `nginx:1.14.2` image with 3 replicas in the local Kubernetes cluster.

DoD:

- You must be able to create the StatefulSet using `kubectl apply` with a YAML configuration file.
- Running `kubectl get statefulsets` should display `my-statefulset` in the list.
- Running `kubectl describe statefulset my-statefulset` should show that the StatefulSet is running 3 replicas of the `nginx:1.14.2` image.

#### Task 1.3.6 Creating a Secret

Create a Secret named `my-secret` with the data `username=admin` and `password=secret` in the local Kubernetes cluster.

DoD:

- You must be able to create the Secret using `kubectl create secret` command.
- Running `kubectl get secrets` should display `my-secret` in the list.
- Running `kubectl describe secret my-secret` should show that the Secret contains the keys `username` and `password`.

#### Task 1.3.7 Creating a ConfigMap

Create a ConfigMap named `my-configmap` with the data `log_level=info` and `max_connections=100` in the local Kubernetes cluster.

DoD:

- You must be able to create the ConfigMap using `kubectl create configmap` command.
- Running `kubectl get configmaps` should display `my-configmap` in the list.
- Running `kubectl describe configmap my-configmap` should show that the ConfigMap contains the keys `log_level` and `max_connections`.

#### Task 1.3.8 Creating a Service

Create a Service named `my-service` that exposes `my-deployment` on port 80 in the local Kubernetes cluster.

DoD:

- You must be able to create the Service using `kubectl apply` with a YAML configuration file.
- Running `kubectl get services` should display `my-service` in the list.
- Running `kubectl describe service my-service` should show that the Service is routing traffic to `my-deployment` on port 80.

#### Task 1.3.9 Creating an Ingress

Create an Ingress named `my-ingress` that routes traffic to `my-service` on path `/` in the local Kubernetes cluster.

DoD:

- You must be able to create the Ingress using `kubectl apply` with a YAML configuration file.
- Running `kubectl get ingress` should display `my-ingress` in the list.
- Running `kubectl describe ingress my-ingress` should show that the Ingress is routing traffic to `my-service` on path `/`.

#### Task 1.3.10 Performing a Rollout Restart

Perform a rollout restart on `my-deployment`.

DoD:

- You must be able to perform a rollout restart on `my-deployment` using the `kubectl rollout restart` command.
- Running `kubectl rollout status deployment my-deployment` should show that the Deployment has been restarted.

#### Task 1.3.11 Patching a Resource

Update the `my-deployment` to use the `nginx:1.16.1` image.

DoD:

- You must be able to update `my-deployment` to use the `nginx:1.16.1` image using the `kubectl set image` command.
- Running `kubectl describe deployment my-deployment` should show that the Deployment is now using the `nginx:1.16.1` image.

#### Task 1.3.12 Creating a Persistent Volume and Persistent Volume Claim

Create a Persistent Volume (PV) named `my-pv` with a capacity of 1Gi and access modes `ReadWriteOnce`. Also, create a Persistent Volume Claim (PVC) named `my-pvc` that requests a volume of 1Gi.

DoD:

- You must be able to create the PV and PVC using `kubectl apply` with a YAML configuration file.
- Running `kubectl get pv` should display `my-pv` in the list.
- Running `kubectl get pvc` should display `my-pvc` in the list.
- The `my-pvc` should be bound to `my-pv`.

#### Task 1.3.13 Updating a Deployment to Use a Persistent Volume

Update `my-deployment` to mount the volume claimed by `my-pvc` at the path `/data`.

DoD:

- You must be able to update `my-deployment` to use the volume claimed by `my-pvc` using `kubectl apply` with a YAML configuration file.
- Running `kubectl describe deployment my-deployment` should show that the Deployment is mounting the volume at `/data`.

#### Task 1.3.14 Creating a Horizontal Pod Autoscaler

Create a Horizontal Pod Autoscaler (HPA) for `my-deployment` that maintains between 1 and 10 replicas and targets CPU utilization at 50%.

DoD:

- You must be able to create the HPA using `kubectl apply` with a YAML configuration file.
- Running `kubectl get hpa` should display the HPA for `my-deployment`.
- Running `kubectl describe hpa my-deployment` should show that the HPA is maintaining between 1 and 10 replicas and targeting CPU utilization at 50%.

#### Task 1.3.15 Creating a Network Policy

Create a Network Policy that allows traffic to `my-deployment` only from Pods in the same namespace.

DoD:

- You must be able to create the Network Policy using `kubectl apply` with a YAML configuration file.
- Running `kubectl get networkpolicies` should display the Network Policy for `my-deployment`.
- Running `kubectl describe networkpolicy my-network-policy` (replace `my-network-policy` with the name of your Network Policy) should show that the Network Policy allows traffic to `my-deployment` only from Pods in the same namespace.

#### Task 1.3.16 Creating a Job

Create a Job that runs the `busybox` image and executes the command `echo "Hello, Kubernetes!"`.

DoD:

- You must be able to create the Job using `kubectl apply` with a YAML configuration file.
- Running `kubectl get jobs` should display the Job.
- Running `kubectl logs job/my-job` (replace `my-job` with the name of your Job) should display "Hello, Kubernetes!".

## Task 2: Pipelines

TODO

### Task 2.1 Jenkins

TODO

### Task 2.2 Gitlab

TODO

### Task 2.3 Github

TODO

## Task 3: Data Formats

TODO

### Task 3.1 JSON

TODO

### Task 3.2 YAML

TODO

### Task 3.3 TOML

TODO

### Task 3.4 XML

TODO

### Task 3.5 CSV

TODO

### Task 3.6 INI

TODO

## Task 4: Infrastructure as Code

TODO

### Task 4.1 Terraform

TODO

### Task 4.2 Ansible

TODO

### Task 4.3 Pulumi

TODO

### Task 4.4 Puppet

TODO

### Task 4.5 Chef

TODO

### Task 4.6 SaltStack

TODO

## Task 5: Cloud Providers

TODO

### Task 5.1 AWS

TODO

### Task 5.2 Azure

TODO

### Task 5.3 GCP

TODO

### Task 5.4 Oracle

TODO

### Task 5.5 Digital Ocean

TODO

### Task 5.6 Linode

TODO

## Questions

Try to answer the following questions with a few sentences:

- TODO

## Terms, buzzwords and more

In order to understand the DevOps (and IT) world, you need to know the following terms, try to copy this table in a markdown file and fill in some information about how you understand the term, if the term has any tools or technologies that you can use for example and if it is not a technology - some use cases:

| Terms, buzzword and more             | Explain in one sentance | Provide example tools, technologies and use cases |
| ------------------------------------ | ----------------------- | ------------------------------------------------- |
| devops pipelines                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| containerization                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| continuous integration               | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| continuous delivery                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| continuous deployment                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| build tools                          | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| container fleet management           | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| version control system               | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| source control system                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| container orchestration              | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| artifact repository                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| AWS EC2                              | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| GCP Compute Instance                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| DevSecOps                            | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| immutable infrastructure             | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| server clustering                    | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| server failover                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| on-premise                           | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| high availability                    | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| configuration management             | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| repository branches                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| application performance monitoring   | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| logs management                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| dynamic scaling servers              | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| infrastructure resilience            | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| UAT                                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| regression testing                   | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| development environment              | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| testing environment                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| environment provisioning             | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| staging environment                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| bastion server                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| bare-metal server                    | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| cloud computing                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| big data                             | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| IaaS                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| PaaS                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| SaaS                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| I/O throughput                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Mean Time to Recovery                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| linux distribution                   | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| rolling update                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| test automation                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| technical debt                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| VPC peering                          | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| software development lifecycle       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| microservices                        | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| monolithic application               | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| type 1 hypervisor                    | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| bootloader                           | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| API                                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| deployment frequency                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| percentage of failed deployments     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| distributed vs decentralized systems | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| continuous monitoring                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| serverless computing                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| RAID                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| script shebang                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| data science                         | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| deep learning                        | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| FOSS/FLOSS software                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Blue/Green deployment                | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| A/B Testing                          | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Canary releases                      | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Rolling releases                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Infrastructure as Code               | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Compliance as Code                   | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Security as Code                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| Pre-commit hooks                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| SAST                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| DAST                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| cloud agnostic                       | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| idempotent resource                  | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| SDLC                                 | [YOUR ANSWER]           | [YOUR ANSWER]                                     |
| tainted resource                     | [YOUR ANSWER]           | [YOUR ANSWER]                                     |

An example of how to fill in data:

| Terms, buzzword and more | Explain in one sentence                                    | Provide example tools, technologies and use cases                                                           |
| ------------------------ | ---------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| devops pipelines         | Automated workflows that orchestrate software delivery.    | Tools: Jenkins, CircleCI, GitLab CI/CD. Use Cases: Continuous delivery, deployment automation.              |
| containerization         | Packaging applications along with their dependencies.      | Technologies: Docker, Kubernetes. Use Cases: Scalable and portable deployments, microservices architecture. |
| continuous integration   | Regularly integrating code changes to detect issues early. | Tools: Travis CI, Jenkins, GitLab CI/CD. Use Cases: Early bug detection, ensuring code quality.             |
