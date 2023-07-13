# Getting Started

Install Docker on your Linux installation by following the official documentation: https://docs.docker.com/engine/install/#server. The easiest way is installing it by using the convenience script:

Run this command in your server (run as root if permissions denied)

```curl -fsSL https://get.docker.com | sudo sh```

Now download and run the start.sh script or just type it in.

> Note: You may be interested in adjusting Nextcloud’s datadir to store the files in a different location than the default docker volume. See this [documentation](https://github.com/nextcloud/all-in-one#how-to-change-the-default-location-of-nextclouds-datadir) on how to do it.

After the initial startup, you should be able to open the Nextcloud AIO Interface now on port 8080 of this server.

E.g. ```http://<ip address>:8080```

So, now after setting and starting up all containers from AIO it could take sometime to download all and start Nextcloud so after that refresh it should look like this:
| First setup | After installation |
|---|---|
| ![image](https://user-images.githubusercontent.com/42591237/232849125-30e24c85-bfd7-465e-8310-9b69cd9666fe.png) | ![image](https://user-images.githubusercontent.com/42591237/232849036-28c38d9a-3151-4cf1-97a5-4d94c1f0eba0.png) |

After all are running you can close this and go towards you Nextcloud:

```http://<ip address>:11000```

### Now you can configure you Nextcloud as per your needs.
