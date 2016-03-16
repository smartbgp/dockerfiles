# dockerfiles

## YABGP

Example

```bash
$ docker run -d -p 8801:8801 -v /var/data/user1:/root/data -e LOCAL_AS=100 -e REMOTE_AS=100 -e REMOTE_IP=10.124.1.221 -e AFI_SAFI=ipv4,ipv6 yabgp:latest
```

You can get the bgp message file and log file in local disk.

``` bash
$ cd /var/data/user1/bgp/10.124.1.221/
$ ls
log  msg
$ cd log
$ ls
yabgp.log
$ cd ../msg/
$ ls
1458116526.06.msg
```

## YABMP

