## SSPanel V3 Mod Backend 

>  *A simple docker image for SSPanel V3 Mod Backend*



### Usage

https://vinga.tech/ssrmu/



### Support ENV

```
NODE_ID=0
DNS_1=1.0.0.1
DNS_2=8.8.8.8
SPEEDTEST=6
CLOUDSAFE=0
AUTOEXEC=0
ANTISSATTACK=0
MU_SUFFIX=zhaoj.in
MU_REGEX=%5m%id.%suffix
API_INTERFACE=modwebapi
WEBAPI_URL=https://zhaoj.in
WEBAPI_TOKEN=glzjin
MYSQL_HOST=127.0.0.1
MYSQL_PORT=3306
MYSQL_USER=ss
MYSQL_PASS=ss
MYSQL_DB=shadowsocks
REDIRECT=github.com
DNS_IPV6=true
CONNECT_VERBOSE_INFO=1
FAST_OPEN=false
```
### docker-compose启动
```
version: '3'

services:
 ssrmu-sspanel:
    image: fanvinga/docker-ssrmu
    restart: always
    network_mode: "host"
    env_file:
      - ./ssrmu-sspanel/config.env
    logging:
      options:
        max-size: "1m"
        max-file: "1"
```

### Thanks to glzjin and the others
