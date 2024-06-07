**Nama** : Fasihul Ilmi </br>
**NRP** : 3122600027 </br>
**Kelas** : 2 D4 IT A </br>

# Konfigurasi MikroTik, DNS Server, Web Server, dan Email Server

### MikroTik
```
{
# jan/02/1970 02:13:29 by RouterOS 6.39.3
# software id = SAKP-Q6US
#
/interface bridge
add name=bridge1
/interface wireless security-profiles
set [ find default=yes ] supplicant-identity=MikroTik
/ip pool
add name=dhcp_pool0 ranges=192.168.8.2-192.168.8.254
/ip dhcp-server
add address-pool=dhcp_pool0 disabled=no interface=bridge1 name=dhcp1
/interface bridge port
add bridge=bridge1 interface=ether10
add bridge=bridge1 interface=ether2
add bridge=bridge1 interface=ether3
add bridge=bridge1 interface=ether4
add bridge=bridge1 interface=ether5
add bridge=bridge1 interface=ether6
add bridge=bridge1 interface=ether7
add bridge=bridge1 interface=ether8
add bridge=bridge1 interface=ether9
/ip address
add address=192.168.88.8/24 interface=ether10 network=192.168.88.0
add address=192.168.8.1/24 interface=bridge1 network=192.168.8.0
/ip dhcp-server network
add address=192.168.8.0/24 dns-server=192.168.8.10 gateway=192.168.8.1
/ip firewall nat
add action=masquerade chain=srcnat dst-address=0.0.0.0/0 src-address=\
    192.168.8.0/24
/ip route
add distance=1 gateway=192.168.88.254
add distance=1 dst-address=192.168.1.0/24 gateway=192.168.88.1
add distance=1 dst-address=192.168.2.0/24 gateway=192.168.88.2
add distance=1 dst-address=192.168.3.0/24 gateway=192.168.88.3
add distance=1 dst-address=192.168.4.0/24 gateway=192.168.88.4
add distance=1 dst-address=192.168.5.0/24 gateway=192.168.88.5
add distance=1 dst-address=192.168.6.0/24 gateway=192.168.88.6
add distance=1 dst-address=192.168.7.0/24 gateway=192.168.88.7
add distance=1 dst-address=192.168.9.0/24 gateway=192.168.88.9
add distance=1 dst-address=192.168.10.0/24 gateway=192.168.88.10

}
```
### DNS Server

