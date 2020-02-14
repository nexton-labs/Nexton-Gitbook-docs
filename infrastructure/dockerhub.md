# DockerHub

DockerHub is the central repository to store container images. We use it, to upload the generated image after a successful build is done. We are not uploading images for every change, just for specific git branches. Usually development and master branches that will be used to be deployed to a development and production environments.

So, one of the first steps to create our continuous delivery pipeline is to create a new repository in docker hub to store our generated images. To do that, we just go to docker hub site:

* Url: [https://hub.docker.com/](https://hub.docker.com/) 
* Username: xxxxxx
* Password: xxxxx

Once we login with the [DockerHub](https://hub.docker.com/) account we can create a new repository for the new application we want to build and push.

For creating a new Repository we have to click the Create Repository button and follow the instructions. ****

![](../.gitbook/assets/image%20%283%29.png)

