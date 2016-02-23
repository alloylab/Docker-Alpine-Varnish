# Varnish Docker container

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