# CircleCI

CircleCI is a continues integration and continues delivery server. There are no credentials available for this service. You just have to login into [CircleCI](https://circleci.com/) using your [GitHub](https://github.com) credentials, it will automatically detect if the logged user has access to the project repository.

When you are dealing with a new project that you want to build, just go to the console, click on the Add project button and you will see a list of all the projects that are not yet integrated with the service

![](https://github.com/nexton-labs/docs/tree/7da9da3c16b52046e57271ac9f6e8f9c76f282e1/.gitbook/assets/image%20%2810%29.png)

Click on Set Up Project and this will send you to a screen to choose in which technology your project was developed and it will show you a config.yml template for that technology

![](../../.gitbook/assets/image%20%284%29.png)

You will need to copy that file and store it in a .circleci folder within your project, before hitting Start Building

Check here for an example [https://github.com/nexton-labs/node-starter/tree/master/.circleci](https://github.com/nexton-labs/node-starter/tree/master/.circleci)

