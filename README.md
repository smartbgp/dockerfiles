# dockerfiles

## YABGP

Example

```bash
docker run -p 8801:8801 -v /home/yabgp/data:/root/data -e LOCAL_AS=100 -e REMOTE_AS=100 -e REMOTE_IP=10.75.44.228 -e AFI_SAFI=ipv4,ipv6  yabgp:latest
```
