# Services

#### **CircleCI**

* Url: [https://circleci.com/](https://circleci.com/) 

There are no credentials available for this service. You just have to login into [CircleCI](https://circleci.com/) using your [GitHub](https://github.com) credentials, it will automatically detect if the logged user has access to the project repository.

**Docker-Hub**

* Url: [https://hub.docker.com/](https://hub.docker.com/) 
* Username: xxxxxx
* Password: xxxxx

Once we login with the [DockerHub](https://hub.docker.com/) account we can create a new repository for the new application we want to build and push to DockerHub.

For creating a new Repository we have to click the Create Repository button and follow the instructions. ****

### **Amazon AWS**

* Url: [https://&lt;accountIdOrAlias&gt;.signin.aws.amazon.com/console](https://nexton.signin.aws.amazon.com/console)
* Account ID or alias: nexton
* IAM user name: xxxx-xxxxxx
* Password: xxxxxx

#### **Elastic Beanstalk \(EBS\)**

Elastic Beanstalk manage applications with environments. To create a new environment, first we need to go to Elastic Beanstalk console.

![](../.gitbook/assets/image.png)

Then, you can create a new Application, or if you already have an application create a new environment within your existent application going to **Actions** -&gt; **Create Environment**, choose the option Web Server and setup the new environment as shown in the following screenshots.

![](../.gitbook/assets/image%20%281%29.png)

![](https://lh4.googleusercontent.com/VJrS44WjT9KZk_KIvCQupif6vkAkNp_qAJHBbL5xMihhUsr_Sd8-YEswQ5MglRel8Z7TCHjhht6XRif_q_iDSbfzb-cRlFDEfunYO-1rj2OHdhDLxjDZ7M6AgOUWCK8zOD4jlR9WQgrKaRCQxA)

![](../.gitbook/assets/image%20%282%29.png)

Note that the preconfigured platform chosen is [Docker](https://www.docker.com/). Also, we have to change the name and the required hardware by clicking Configure more options.

#### **S3 \(Storage\)**

![](https://lh3.googleusercontent.com/nY4BSX0mGM6DolM8cUt-g7sygFIvZBwcKv9PEZCswoDMJOzj8taUvtcmim3E7YDGrHKIj32f4Pgcf5TtUDeXPCWVZ0NB0o7Sdrapd524i5X46HeA0wHEsRdIogB_F_7DYOkUOSgm)

The storage is used to save the dockerrun auto-generated files of each deployment, and also contains sensible configuration data to access [DockerHub](https://hub.docker.com/) \(docker/config.json\).  
****

