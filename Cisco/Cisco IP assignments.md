IPV4 
config terminal
interface <name>
ip address <ipv4 address, subnet mask>

IPV6
config terminal 
interface <name>
ipv6 address <ipv6 address> /64 (or relevant /notation, IOS will reject if incorrect syntax)

ipv6 will apply the configured address as  well as a link-local address
the link-local can be assigned manually

ipv6 address <ipv6 addres> link-local

