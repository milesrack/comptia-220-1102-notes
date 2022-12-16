## ipconfig
- `ipconfig`
- Adapter and IP information (IPv4 and IPv6)
- View DNS server, DHCP server, etc.
- `ipconfig /all` shows more extensive information
## ping
- `ping`
	- `ping 9.9.9.9`
- Test reachability
- Determine round-trip time
- Uses ICMP (Internet Control Message Protocol)
## netstat
- `netstat`
- Network statistics
- Windows, MacOS, and Linux
- `netstat -a`
	- All active connections
- `netstat -b`
	- Shows binaries (Windows)
	- Needs elevation
- `netstat -n`
	- Don't resolve names
## nslookup
- `nslookup`
- Name server lookup
- Looks up info from DNS servers
	- Canonical names, IP, cache timers, etc.
## net
- Windows network commands
- Network resources
	- `net view \\<servername>`
	- `net view /workgroup:<workgroupname>`
- Map netowkr share
	- `net use <drive>: \\<servername>\<sharename>`
- View user account info
	- `net user <username>`
	- `net user <username> * /domain`
## tracert
- `tracert`
- Uses ICMP
- Takes advantage of TTL exceder error message
	- TTL = hops , not seconds/mins
	- TTL=1 is first router, TTL=2 is seconds, etc.
- Determine route a packet takes
- Each router that recieves packet decreases TTL by 1
- Some devices will not reply with ICMP time exceeded
	- Firewall rules
	- ICMP is low-priority on most devices
## pathping
- `pathping`
- Combines ping and traceroute
- First phase runs traceroute to build map
- Second phase measures round trip time and packet loss at each hop