# Varnish Docker Container

[![](https://badge.imagelayers.io/alloylab/varnish:latest.svg)](https://imagelayers.io/?images=alloylab/varnish:latest)

> Alpine Lastest  
> Varnish 4.x

## Usage

Default VCL forwards port 80 traffic to port 8080

```
docker run --detach \
--publish 80:80 \
--name varnish \
--restart always \
-i -t \
alloylab/varnish;
```

Also add one of the following so the Container knows where to send the traffic,
--link web1:web1 \
--env='VARNISH_BACKEND_ADDRESS=192.168.1.1' \