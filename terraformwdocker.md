# Day 68 -  Deploying a Docker container with Terraform

In this task, You will learn how to deploy a Docker container using Terraform. You have to use the Docker provider for Terraform to create and manage the container.


## Task-01: Terraform with Docker
Terraform needs to be told which provider to be used in the automation, hence we need to give the provider name with source and version.
For Docker, we can use this block of code in your main.tf
```
terraform {
  required_providers {
    docker = {
      source  = "kreuzwerker/docker"
      version = "~> 2.21.0"
}
}
}

```
Note: kreuzwerker/docker, is shorthand for registry.terraform.io/kreuzwerker/docker.


## Provider
The provider block configures the specified provider, in this case, docker. A provider is a plugin that Terraform uses to create and manage your resources.
provider "docker" {}

## Resource
Use resource blocks to define components of your infrastructure. A resource might be a physical or virtual component such as a Docker container, or it can be a logical resource such as a Heroku application.
Resource blocks have two strings before the block: the resource type and the resource name. In this example, the first resource type is docker_image and the name is Nginx.
```
resource "docker_image" "nginx" {
 name         = "nginx:latest"
 keep_locally = false
}

resource "docker_container" "nginx" {
 image = docker_image.nginx.latest
 name  = "tutorial"
 ports {
   internal = 80
   external = 80
 }
}
```

Don't forget to post your progress on Linkedin. Till then Happy learning :)
