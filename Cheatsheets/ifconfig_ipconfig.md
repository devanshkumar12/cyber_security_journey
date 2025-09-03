# 🖥️ Networking Commands Cheatsheet  

## 🔹 Linux (ifconfig / ip)  
- `ifconfig` → Show IP, MAC, and network info (deprecated, but still used).  
- `ifconfig eth0 down` → Disable network interface.  
- `ifconfig eth0 up` → Enable network interface.  
- `ifconfig eth0 192.168.1.10` → Assign IP to interface.  
- `ifconfig eth0 netmask 255.255.255.0` → Set subnet mask.  
- `ifconfig eth0 broadcast 192.168.1.255` → Set broadcast.  
- `ifconfig eth0 mtu 1000` → Set MTU size.  
- `ip addr` → Show all interfaces & IPs.  
- `ip link show` → Show all network interfaces.  
- `ip link set eth0 down` → Disable interface.  
- `ip link set eth0 up` → Enable interface.  
- `ip addr add 192.168.1.100/24 dev eth0` → Add IP to interface.  
- `ip route show` → Show routing table.  
- `ip route add default via 192.168.1.1` → Add default gateway.  

---

## 🔹 Windows (ipconfig)  
- `ipconfig` → Show IP, subnet mask, default gateway.  
- `ipconfig /all` → Show full details (DNS, MAC, DHCP).  
- `ipconfig /release` → Release current IP.  
- `ipconfig /renew` → Renew IP from DHCP.  
- `ipconfig /flushdns` → Clear DNS cache.  
- `ipconfig /displaydns` → Show DNS cache.  

---

## 🔹 Extra Commands (Both)  
- `ping` → Test connectivity.  
- `tracert` (Windows) / `traceroute` (Linux) → Trace path to host.  
- `nslookup` → Get DNS info.  
- `netstat -ano` → Show active connections & ports.  
- `arp -a` → Show ARP table (IP ↔ MAC mapping).  
