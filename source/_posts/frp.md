---
title: frp
date: 2023-07-10 12:21:34
tags: [linux,docker,frp]
---

# frp docker deployment

## official docs

https://gofrp.org/docs

## before the work

frp contains two parts: the server and the client.

Server (frps) is meant to run on an instance with public ip address.
Client (frpc) is meant to run on any instance that needs to expose ports for its services.

Take SSH for example, if you have a VM instance that is running in your private network with ip address 192.168.0.55, you need to expose its SSH service to public.

You need to deploy frpc on this VM instance. When frpc is running on this VM, it will talk with Server (frps) that is running on the instance with public ip address.

Then when you need to SSH to this VM instance, you dont have to connect to its private address 192.168.0.55 directly, which will not work. Instead, you need to connect to the Server (frps) on specified port, then frps will reverse proxy the data to that VM instance.

## frps setup

- frps.yml

```yml
version: "3.3"
services:
  frps:
    #restart: always
    image: "snowdreamtech/frps:latest"
    container_name: frps
    network_mode: "host" # linux only, windows does not support
    volumes:
      - ./frps.ini:/etc/frp/frps.ini
```

here network_mode = host is used, which mean windows will not support this option.

- frps.ini

```ini
[common]
bind_port = 7000
dashboard_port = 7500
token = <token> # should be same as frpc
dashboard_user = <user>
dashboard_pwd = <pwd>
```

### frpc setup

```yml
version: "3.3"
services:
  frpc:
    image: stilleshan/frpc
    container_name: frpc
    #restart: always
    network_mode: "host" # linux only, windows does not support
    volumes:
      - ./etc/frp/frpc.ini:/frp/frpc.ini
```

here network_mode = host is used, which mean windows will not support this option.


```ini
[common]
server_addr = <your public ip address>
server_port = 7000
tls_enable = true
token = <token> # should be same as frps

[ssh]
type = tcp
remote_port = 8222
local_ip = localhost
local_port = 22
```

## use

- start frps first on your instance that has public ip address
- then start frpc on your instance that has private ip address
- ssh yourname@<your public ip address> -p 8222 will actually ssh connected to your private VM instance.


