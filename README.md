# Local Proxy

This is [dinghy-http-proxy](https://github.com/codekitchen/dinghy-http-proxy) docker-compose setting for development using Docker for Mac.

## How to use

```
docker-compose up -d
```


## SSL setting
same as dinghy-http-proxy.
just put your certificates and privates keys in the `HOME/.dinghy/certs` directory for any virtual hosts in use. 

## DNS setting


create a file `/etc/resolver/docker` (creating the `/etc/resolver` directory if it does
not exist) with these contents:

```
nameserver 127.0.0.1
port 19322
```

Docker for Mac uses `127.0.0.1` as the IP.

## Others

see [dinghy-http-proxy](https://github.com/codekitchen/dinghy-http-proxy).
