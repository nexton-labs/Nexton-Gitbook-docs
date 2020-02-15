# Databases

For databases, what we usually use is AWS RDS DBs, as with this AWS service we have a couple of features being handled automatically, like:

* DB configuration
* Patching
* Automatic backups

So, to start with DB creation, go to RDS in AWS console and click on create database. First step would ask you what type of DB you would like to create, choose the one that adjust to your environment needs.

![](../.gitbook/assets/image%20%2813%29.png)

For license model and engine version, try to choose the las supported version if your application is compatible with it:

![](../.gitbook/assets/image%20%282%29.png)

**Note:** In case you are creating a DB for a POC app, you can choose the option to only enable options eligible for RDS Free tier

Then, you will need to choose the DB instance class. Here you will need to consider the amount of [memory and cpu](https://docs.amazonaws.cn/en_us/AmazonRDS/latest/UserGuide/Concepts.DBInstanceClass.html) that your DB will need for your app, but also, take into account some other configurations like [encryption](https://docs.amazonaws.cn/en_us/AmazonRDS/latest/UserGuide/Overview.Encryption.html).

For this example we will create a t2.micro DB, encryption cannot be enabled on this type of RDS class.

![](../.gitbook/assets/image%20%2815%29.png)

Multi-AZ deployment will be a great feature to have when you are configuring a Production environment where you expect to have high data loads.

Storage autoscaling, we left it as default.

![](../.gitbook/assets/image%20%2811%29.png)

Then you need to set the DB instance identifier, that is the DB RDS resource name that AWS will use, and the master user name that is the name of the user you will use to access the Database

![](../.gitbook/assets/image%20%2819%29.png)

Now, we need to configure networking and security. **An important point here is to create the DB as private**. This means that you will not be able to connect directly to it, you will need to use a jump server. This jump server would be an EC2 instance running on the same AWS account. You can check more details on how to connect to the DB [here](https://medium.com/nexton/how-to-make-your-amazon-rds-db-private-if-its-already-public-c37bf9d6f544).

![](../.gitbook/assets/image%20%281%29.png)

Following with the rest of the configuration, you will see that for this type of DB class, we are not allowed to enable encryption:

![](../.gitbook/assets/image%20%286%29.png)

Then, you left all the next configuration settings as default and click on create database

![](../.gitbook/assets/image%20%2816%29.png)

![](../.gitbook/assets/image%20%288%29.png)

![](../.gitbook/assets/image%20%285%29.png)

![](../.gitbook/assets/image%20%2817%29.png)

![](../.gitbook/assets/image%20%287%29.png)

Note: Enable deletion protection is recommended for Production DBs. Anyways, you will always have daily snapshots to recover in case of any issues.

