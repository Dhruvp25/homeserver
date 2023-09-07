<p align="center">
  <img src="https://raw.githubusercontent.com/immich-app/immich/main/design/immich-logo.svg" width="150" alt="Login With Custom URL">
</p>
<h3 align="center">Immich - High performance self-hosted photo and video backup solution</h3>
<br/>
<a href="https://immich.app">
<img src="https://raw.githubusercontent.com/immich-app/immich/main/design/immich-screenshots.png" title="Main Screenshot">
</a>
<br/>

## Documentation

You can find the main documentation, including installation guides, at https://immich.app/.

## Github Page

You can find whole project by the Creater here  [Immich Github](https://github.com/immich-app/immich)

### Here are the steps that I have taken to create and implement the Immich app on my server.

You can visit [here](https://immich.app/docs/install/script) and check out all steps by Creater or just follow me simple.

### Step 1

In the shell, from a directory of your choice, run the following command:

```
curl -o- https://raw.githubusercontent.com/immich-app/immich/main/install.sh | bash
```

> The script will perform the following actions:

1. Download docker-compose.yml, and the .env file from the main branch of the repository.
2. Populate the .env file with necessary information based on the current directory path.
3. Start the containers.

The web application will be available at:
```
http://<your-ip-address>:2283
```

> The directory which is used to store the library files is ./immich-data relative to the current directory.

### Step 2

Reverse-proxy it by your domain with help of cloudflared services.

> Make tunnel as name by
```
photos.yourdomain.com
```

**You Can Visit and Setup your Photos app at you link above and Get Started.**

## Step 3

Upgrading

If ```IMMICH_VERSION``` is set, it will need to be updated to the latest or desired version.

And in our case we need to upgrade our immich app as new releases come often

So Just " cd " to your desired folder where you had the immich directory and in that you can see you ```docker-compose.yml``` file.

> In that use the following command to upgrade and update your immich app:
```
docker-compose pull && docker-compose up -d     # Or `docker compose up -d`
```
