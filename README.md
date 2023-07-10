# Home Server
This repository is specially for Home server setup using Ubuntu Linux.

Here I have whole setup of zero to advanced Home Server, where i have used several apps and installer's to make a perfect Server hosted from your home with very low rated trash pc with some **PC Specs** down below:
- Intel Pentium inside G620
- 2G + 8G RAM sticks (1333Mhz DDR3)
- 1Tb + 500Gb HDD (seagate baracuda)

Here I have also mentioned some prerequistics needed to deploy this whole home server:
* Ethernet Internet connection to Server (PC)
* Wired keyboard
* Moniter screen to install ubuntu server
* 4+ GB Pendrive


## Let's Get Started as we are all set to Install and Start our own Home Server.
> You also need some knowledge in Coding and linux to configure things yourself.

### Step 1

Downloading Ubuntu server from the link : 
```https://ubuntu.com/download/server```

Install [Ventoy](https://www.ventoy.net/en/download.html) on your windows device, using ventoy make our pendrive a bootable drive by selecting it and installing ventoy on it
Move Ubuntu server .ISO file on our USB drive.
As we need to install ubuntu server on our server via bootable drive we did this process, so now inserting it in the server and Starting it for the first time, we need to select our boot device from the boot menu on startup so every system motherboard has different keys assigned to select the boot device menu on startup so look for it on the internet as per your System needs.
> In my case it was F10 to select boot device.

- Select our boot device (USB drive) and Enter
- It will open the ventoy menu to slect which .iso file to run to install it on server
- We'll select Ubuntuserver.iso and it will start installing ubuntu server.
- Now dont remove USB Drive untill end

### Step 2

As our Ubuntu interface would look like this:

![ubuntu server starting page](https://ubuntucommunity.s3.dualstack.us-east-2.amazonaws.com/original/2X/9/92bda8a0ed1ed1ac3137015191ee81e69c38ff3d.png)

Now go on [Ubuntu Installation](https://ubuntu.com/server/docs/install/step-by-step) guide to get a step by step guide to install whole ubuntu server.

Here is some help if needed:
* continue without updating
* make sure you have ethernet cable connected to the server, so next it will show you your IP
* skip proxy address
* skip mirror address
* Now for **[Storage](https://ubuntu.com/server/docs/install/storage)** you need to configure your's as per your storage avaibility and needs mine look like's this
 
![My Storage config](https://github.com/Dhruvp25/homeserver/assets/71492443/c3aaa141-868b-4f99-8814-92dfe6cdd2f8)

* And after confirming storage configuration
* You'll need to Setup your "NAME" , "SERVER NAME" , "USER NAME" (to login with it in our server) , "PASSWORD" (root password so make it strong)
* Select Yes for [X] Install openSSH server
* Don't select any snaps as we'll install them later as per our need and in easy way.
* Now at last **DONE** and it will start installing our server.
* after installing it will give **reboot** option select that and straight away it will tell you to remove installation drive (USB Drive)
* And after doing all Correctly our server should start in a perfect way. (first time loading could take some time)

## Our Homer server is all set to serve us as we deploy our services.
