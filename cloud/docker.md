# Docker Related Articles, Things To Try

I'm making some progress incorporating more Docker into my daily workflows.
I keep forgetting some commands, so here it's gonna be my memo block:

## Useful Commands

| Command                          | Description                                            |
| ---                              | ---                                                    |
| `docker images`                  | Get the list of local images                           |
| `docker rmi <image>`             | Remove local image by name or ID                       |
| `docker rmi -f <image>`          | Force remove local image by name or ID                 |
| `docker run .. --name <name>`    | --name - gives name to container - good practice       |
| `docker run -it <image>`         | -i - interactive -t - TTY - get the shell running      |
| `<Ctrl-P-Q>`                     | To exit interactive shell, but container keeps running |
| `docker ps`                      | List of running containers                             |
| `docker attach <container_name>` | Attach to running container                            |
| `docker rm <container_name>`     | Kill running container                                 |
| `docker rm -f <container_name>`  | Force kill running container                           |

## Dockerize your app and keep hot-reloading!
https://blog.bam.tech/developper-news/dockerize-your-app-and-keep-hot-reloading

Pretty random article, one of many I want to check on the Docker usage.

## Fast development workflow with Docker and Kubernetes
https://dev.to/datawireio/fast-development-workflow-with-docker-and-kubernetes-1if

Development setup. Kubernetes part is interesting to study.

## Rails on Docker: Using Docker Compose with Your Ruby on Rails Apps
https://www.chrisblunt.com/rails-on-docker-using-docker-compose-with-your-ruby-on-rails-apps/

Another article how to use Docker. I'm not perticularly interested in RoR, but
I'm hoping that this article will help me understand some mechanics of Docker usage.

## Developing Microservices - Node, React, and Docker 
http://mherman.org/blog/2017/05/11/developing-microservices-node-react-docker/#.WkhZnCOZP6D

In this post you will learn how to quickly spin up a reproducible development environment with Docker 
to manage a number of Node.js microservices.

## Try C++17 with Docker
http://www.jandeinhard.de/2017/09/15/cpp-and-docker.html

I'm going after 2 things here - Docker and actually trying C++17 and GCC.

## Clang 5 in a Docker container for C++17 development
https://solarianprogrammer.com/2017/12/14/clang-in-docker-container-cpp-17-development/?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%3A+SolarianProgrammer+%28Solarian+Programmer%29

Pretty similar to previous article, using Clang 5.

## Docker CLI commands and what you can do with them
http://dev.to/twaintaylor/docker-cli-commands-and-what-you-can-do-with-them-5dg3

## An Exhaustive Guide to Writing Dockerfiles for Node.js Web Apps
https://blog.hasura.io/an-exhaustive-guide-to-writing-dockerfiles-for-node-js-web-apps-bbee6bd2f3c4

Introductory article that explain basic docker commands.

## Why to Docker Compose your developer environment
https://dev.to/danlebrero/why-to-docker-compose-your-developer-environment

Docker Compose introductory.

## Docker Swarm Concepts, Tips, and Tricks for a Docker Beginner
https://dev.to/limiw/docker-swarm-concepts-tips-and-tricks-for-a-docker-beginner-4j4h

Fairly short article about Docker Swarm.

## Kubernetes: It's alive!
https://dev.to/danielkun/kubernetes-its-alive-2ndc

## Deploying to Google Kubernetes Engine
https://codeascraft.com/2018/06/05/deploying-to-google-kubernetes-engine/

## A checklist for Docker in the Enterprise
https://zwischenzugs.com/2016/07/08/a-checklist-for-docker-in-the-enterprise/

Pretty famous checklist about usage of Docker in production.

## Static code analysis in 3 steps
https://dev.to/rafalpienkowski/static-code-analysis-in-3-steps-2ahi

Another docker image usage.

## Docker On Windows

This series of links are about specifics of running Windows Docker images.

### Installing Build Tools for Visual Studio 2017 in a Docker container
https://blogs.msdn.microsoft.com/heaths/2017/09/18/installing-build-tools-for-visual-studio-2017-in-a-docker-container/

Microsoft articles that shows how to setup VS2017 build tools in Docker.
Could be useful to build image for building instance.

### .NET Microservices. Architecture for Containerized .NET Applications
https://docs.microsoft.com/en-us/dotnet/standard/microservices-architecture/

Microsoft eBook about containers in Windows.

### How to install DirectX to Windows Server Core (docker container)
https://social.msdn.microsoft.com/Forums/sqlserver/en-US/386adbc4-3e43-4896-8cbb-ba9cc7fc6b72/how-to-install-directx-to-windows-server-core-docker-container?forum=windowscontainers

Discussion about installing DirectX in Windows Docker image.

### How to Dockerize Windows Applications
https://blog.sixeyed.com/how-to-dockerize-windows-applications/










