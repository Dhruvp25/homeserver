# Deploying PORTAINER

To Deploy PORTAINER on you ubuntu server you need to run the following docker.yml code in your server terminal as a root.

Here we also want it to run on http so we alsos hve included ```-p 9000:9000``` in our command so that it can also be hosted on http port.

Now that the installation is complete, you can log into your Portainer Server instance by opening a web browser and going to:

```http://localhost:9443```

or

```http://localhost:9000```
Replace ```localhost``` with the Our server IP address, and adjust the port if you changed it earlier.

>You will be presented with the initial setup page for Portainer Server.


![](https://2914113074-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FiZWHJxqQsgWYd9sI88sO%2Fuploads%2FG988U9V4JNmqPglD13A6%2F2.15-install-server-setup-user.png?alt=media&token=435a7916-0e9f-4d88-bf22-cc5fa467d9b0)
