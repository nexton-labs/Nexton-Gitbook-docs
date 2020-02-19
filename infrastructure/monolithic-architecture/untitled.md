# Introduction

The main idea of this document is to present how we implement [Continuous Deployment](https://www.agilealliance.org/glossary/continuous-deployment/) in Nexton.

There are four different services that we need to integrate:

* [CircleCI](https://circleci.com/): the [continuous integration](https://en.wikipedia.org/wiki/Continuous_integration) and delivery platform
* [Docker](https://docker.com/) & [Docker-Hub](https://hub.docker.com/): Docker is a set of tools for creating and running the application in containers, and it isolates the application from all the other software running on a server. Docker Hub is the repository for the container images.
* [AWS Elastic Beanstalk](https://aws.amazon.com/ElasticBeanstalk):  Amazon orchestration service that is being used to deploy applications that use several AWS services\(EC2, RDS, S3, etc\) .
* [AWS S3](https://aws.amazon.com/s3/): Amazon storage service.

The flow explained simply:

The process starts with a push to a specific [GitHub branch](https://guides.github.com/introduction/flow/). Once we push something new to [GitHub](https://github.com), [CircleCI](https://circleci.com/) is triggered and runs the Continuous Integration steps specified on the circle.yml file.

If we have a green build, [CircleCI](https://circleci.com/) also creates a Docker image and push it to the [DockerHub](https://hub.docker.com/) repository. Finally, we have to inform AWS that a new Docker image is available so it can be deployed into Amazon.  


