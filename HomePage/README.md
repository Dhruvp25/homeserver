# Get started by going to [Homepage](https://gethomepage.dev/installation/docker/)

### With Docker

Installing it with Docker Compose
```yaml
version: "3.3"
services:
  homepage:
    image: ghcr.io/benphelps/homepage:latest
    container_name: homepage
    ports:
      - 3000:3000
    volumes:
      - /path/to/config:/app/config # Make sure your local config directory exists
      - /var/run/docker.sock:/var/run/docker.sock:ro # (optional) For docker integrations
```
or docker run:

```bash
docker run -p 3000:3000 -v /path/to/config:/app/config -v /var/run/docker.sock:/var/run/docker.sock ghcr.io/benphelps/homepage:latest
```

So, After installation the homepage site will be available for you on http://<ip.address>:3000

## Configuration

Configuration files will be generated and placed on the first request.

Configuration is done in the /config directory using .yaml files. Refer to each config for
the specific configuration options.

You can also check [the homepage site](http://gethomepage.dev) for detailed configuration instructions.

### My Config files

In config folder my files can help to figure out how to setup all things as my home page below:

![hompage](https://github.com/Dhruvp25/homeserver/assets/71492443/1de94256-1115-4b79-abc4-ceddfea8367a)
