# docker-oracle-ee-12c
Oracle 12c Enterprise Edition 12.2.0 and MongoDB 4 in Docker


# To download the image with docker 

`docker pull wxkin/oracle-12c-mongo4`

# If you need a proxy configuration:
`sudo mkdir /etc/systemd/system/docker.service.d`

Create file `/etc/systemd/system/docker.service.d/http-proxy.conf` with the following content:

```
[Service]
Environment="HTTP_PROXY=http://127.0.0.1:3128/"
```

Flush changes:
`$ sudo systemctl daemon-reload`

Restart Docker:
`$ sudo systemctl restart docker`
