# Packet Support

Launch a Type-0, Type-1 or Type-3 Ubuntu 14.04 server and use the below cloud config.  You can add any additional RancherOS configuration to it, but below is the bare minimum you need to provision RancherOS.

```yaml
#cloud-config
runcmd:
- wget -O /tmp/cc https://raw.githubusercontent.com/rancher/os/v0.4.5-dev-1/scripts/hosting/packet/packet.sh
- bash -x /tmp/cc
```
