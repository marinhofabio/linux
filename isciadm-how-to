```
######  -  sysctl.conf  - ###### 
net.ipv4.conf.all.arp_ignore=1
net.ipv4.conf.all.arp_announce=2
net.ipv4.conf.all.rp_filter=2
```

```
$ sudo iscsiadm -m iface -I em3 -o new 
```

```
$ sudo iscsiadm -m iface -I em4 -o new 
```

```
$ sudo iscsiadm -m iface -I em3 --op=update -n iface.net_ifacename -v em3
```

```
$ sudo iscsiadm -m iface -I em4 --op=update -n iface.net_ifacename -v em4
```

```
$ sudo iscsiadm -m discovery -t st -p 10.255.50.10:3260 -d 8
```

```
$ sudo iscsiadm -m discovery -t st -p 10.255.50.10:3260
```

```
$ sudo iscsiadm -m discovery -t st -p 10.255.50.10:3260 --interface em3
```

```
$ sudo iscsiadm -m discovery -t st -p 10.255.50.10:3260 --interface em4
```

```
$ sudo iscsiadm –m node –u
```

```
$ sudo iscsiadm –m node –l
```

```
$ sudo multipath -ll
```

```
$ sudo systemctl status multipath
````

```
defaults {
        user_friendly_names yes
}
blacklist {
        devnode "^(ram|raw|loop|fd|md|dm-|sr|scd|st)[0-9]*"
        devnode "^hd[a-z]"
        devnode "^sda"
        devnode "^cciss!c[0-9]d[0-9]*"
}
devices {
     device {
          vendor                  "EQLOGIC"
          product                 "100E-00"
          path_grouping_policy    multibus
          features                "1 queue_if_no_path"
          path_checker            readsector0
          path_selector           "round-robin 0"
          failback                immediate
          rr_min_io               10
          rr_weight               priorities
     }
}
```

```
$ sudo systemctl restart multipath.conf
```

