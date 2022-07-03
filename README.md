##### This is a fork of :
https://github.com/lmenezes/cerebro
#### Cause i got tired of warnings and container hanging
####
cerebro-m1
--------------

[![Docker Pulls](https://img.shields.io/docker/pulls/tomthecat/cerebro-m1.svg)](https://hub.docker.com/r/tomthecat/cerebro-m1)

Images are periodically uploaded in [tomthecat/cerebro-m1](https://hub.docker.com/r/tomthecat/cerebro-m1/) docker hub repo.

### Usage

For using latest cerebro-m1 execute:

```
docker run -p 9000:9000 tomthecat/cerebro-m1:0.1a <= This is the only version as 23-03-2023
```

### Configuration

You can configure a custom port for cerebro by using the `CEREBRO_PORT` environment variable. This defaults to `9000`.

**Example**

docker run -e CEREBRO_PORT=8080 -p 8080:8080 tomthecat/cerebro-m1

To access an elasticsearch instance running on localhost:

docker run -p 9000:9000 --network=host tomthecat/cerebro-m1

docker run -ti --rm -p 9000:9000 tomthecat/cerebro-m1:0.1a