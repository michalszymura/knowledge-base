`/etc/freeradius/3.0/clients.conf`
```
client 10.0.0.237 {
	ipaddr = 10.0.0.237
	shortname = ap
	secret = asdfghjkl
}
client 0.0.0.0/0 {
	shortname = anything
	secret = asdfghjkl
}
```
`/etc/freeradius/3.0/users`
```
device-mac-address Cleartext-Password := "device-mac-address"
        Tunnel-Password = per-device-pass,
        Tunnel-Private-Group-ID = "111",
        Fall-Through = Yes

#DEFAULT        Cleartext-Password :="%{User-Name}"
DEFAULT Auth-Type := Accept
        Tunnel-Password = default-password,
        Tunnel-Type = "VLAN",
        Tunnel-Medium-Type = "IEEE-802",
        Tunnel-Private-Group-ID = "107",
        Fall-Through = Yes

```

