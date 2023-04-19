***
`/etc/config/wireless`
 Add to `wifi-iface` section
```
option ppsk '1'
option auth_server 'server-ip'
option auth_secret 'auth-secret'
option dynamic_vlan '2'
option vlan_tagged_interface 'eth0'
option vlan_bridge 'br-vlan'
option vlan_naming '0'
```
***
