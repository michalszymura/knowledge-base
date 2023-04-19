Accept both Tag and Untag traffic on a port

Example of removing untagged vlan and setting everything for dual-mode:
```
vlan 111
no untagged ethernet 1/1/1
tagged ethernet 1/1/1
exit
interface ethernet 1/1/1
dual-mode 111
exit
```
Later we can add other tagged vlans:
```
vlan 107
tagged ethernet 1/1/1
exit
```
