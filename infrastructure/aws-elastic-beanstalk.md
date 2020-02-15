# AWS Elastic Beanstalk

AWS Elastic Beanstalk is an orchestration service offered by Amazon Web Services for deploying applications which orchestrates various AWS services, including EC2, S3, Simple Notification Service, CloudWatch, autoscaling, and Elastic Load Balancers.

We use this service to deploy our containerized applications. Elastic Beanstalk manage applications with environments. To create a new environment, first we need to go to Elastic Beanstalk console.

![](../.gitbook/assets/image%20%2812%29.png)

Then, you can create a new Application, or if you already have an application create a new environment within your existent application going to **Actions** -&gt; **Create Environment**, choose the option Web Server and setup the new environment as shown in the following screenshots.

![](../.gitbook/assets/image%20%2822%29.png)

![](https://lh4.googleusercontent.com/VJrS44WjT9KZk_KIvCQupif6vkAkNp_qAJHBbL5xMihhUsr_Sd8-YEswQ5MglRel8Z7TCHjhht6XRif_q_iDSbfzb-cRlFDEfunYO-1rj2OHdhDLxjDZ7M6AgOUWCK8zOD4jlR9WQgrKaRCQxA)

![](../.gitbook/assets/image%20%285%29.png)

Note that the preconfigured platform chosen is [Docker](https://www.docker.com/). Also, we have to change the name and the required hardware by clicking Configure more options.

