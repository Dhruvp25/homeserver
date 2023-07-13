# Commands

## Update Ubuntu & Install Dependencies

Begin by running the following commands as a root user to update your package listings and install Plex Server dependencies:

```sudo apt update && sudo apt upgrade -y```

```sudo apt install apt-transport-https curl wget -y```

## Install Plex Server

### Import GPG Key:

```sudo wget -O- https://downloads.plex.tv/plex-keys/PlexSign.key | gpg --dearmor | sudo tee /usr/share/keyrings/plex.gpg```

### Import Repository:

```echo deb [signed-by=/usr/share/keyrings/plex.gpg] https://downloads.plex.tv/repo/deb public main | sudo tee /etc/apt/sources.list.d/plexmediaserver.list```

### Refresh Repository:

```sudo apt update```

### Install:

```sudo apt install plexmediaserver -y```

Verify the status of Plex Server services using the systemctl command:

```systemctl status plexmediaserver.service```

If this shows us Active then its great, our services are running perfectly adn if not then make sure you did all things as shown in the above steps.

## Configure Firewall

Check Firewall Status:

```sudo ufw status```

Enable Firewall:

```sudo ufw enable```

> Type “y” as the response.

Enable Port 32400 for Plex Server Service outside access:

```sudo ufw allow 32400```

Enable Port 22 for OpenSSH:

```sudo ufw allow OpenSSH```

## Testing Plex Server

Now you can access the Plex Media Server by accessing the localhost or IP address in your web browser.

```http://<ip address>:32400/web```

If not working you can follow tutorial by Josh. Very well explained
[Plex Media Server | Install on Ubuntu 22.04 LTS](https://www.youtube.com/watch?v=QEP5Tq78cHw)
