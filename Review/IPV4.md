32bit addresses, 4 octets of bits
11111111.11111111.11111111.11111111
notated in decimal 
255.255.255.255
IPv4 Class
A 1.0.0.0 - 127.255.255.255 (/8)  
B 128.0.0.0 -191.255.255.255 (/16)
C 192.0.0.0- 223.255.255.255
--- Reserved ------
--- Multicast -----
D 224.0.0.0 - 239.255.255.255
--- Experimental --
E 240.0.0.0- 255.255.255.255

CIDR "/ notation" expresses number of bits in network portion of address

Reserves
10.0.0.0 (Private Class A)
127.0.0.0 (loopback)
172.16.0.0 (Private Class B)
192.168.0.0
Subnets "Borrows bits"
Network address
[255.255.255].0
11111111.11111111.11111111.[00000000]
                        Usable host addresses
255.255.255.128 
11111111.111111111.11111111.1[0000000]
                        Usable address space
                        Subnet mask "0"s are allowed to be used by hosts
192.168.1.0/24 1-254 usable addresses (00000001) - (11111110)
Last host address used for  broadcast address (11111111)

In /24 i.e 192.168.1.0/24
First address (.0)
Last usable host Address  (.254)
Broadcast: Last Address + 1 (.255),end of host address space

192.168.1.0/25 (255.255.255.128) 255-128 = 127 <= quick broadcast address  (255-x = broadcast) where x = subnet mask byte
first .0, last usable .126 broadcast .127
second subnet
192.168.1.128/25 
first .129, last usable .254, broadcast 255
[subnet cheat sheet](https://www.aelius.com/njh/subnet_sheet.html)
[subnetting practice](https://www.nybi.org/subnet-1.php)

practice and drill in common values, all values are binary from 256

(255.255.255.0)/24 256 addresses
(255.255.255.128)/25 128 addresses
(255.255.254.0)/23 512 addresses
usable host addresses = total addresses minus 2 (network# and broadcast# at start and end of subnet)
