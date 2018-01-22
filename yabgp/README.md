# yabgp container

```
$ docker run -d -p 8801:8801 -v /var/data/user1:/root/data --name bgp smartbgp/yabgp:{tag}--bgp-local_as=100 --bgp-remote_as=100 --bgp-remote_addr=192.168.1.1
```