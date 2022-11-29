IPV6 hex notation
0-F
64 bit addresses instead of 32, 8 octets of 8 bits in binary
use hex notation to shorten into 8 "quartets"
9000:A000:0B00:000C:0000:0000:E000:F000 /64

still uses /notation
[9000:000A:0B00:000C] :0000:0000:E000:000F /64
Network address portion, is the first 64 bits
each digit representing 2 bits (16 possible values 0-F)
can shorten notation by clearing leading   0s from notation
any sections of only 0 can be omitted leaving only colons (:) Consecutive 0 sections can be  assumed based on number of visible quartets to total 8 sections
9000:A:B00:C::E000:F
Following 0s must remain as they hold place and remain significant digits

# *casts
## Unicast
Direct sender-to-receiver 

"Unspecified Unicast" default routing protocol, noted as "::/128" or just "::"

Loopback for testing, ::1/128

Unique local unicast FC00::/7, similar to IPv4 private addressing

Global  Unicast 2000-3FFF/3, used for internet routing

Link-local Unicast FE80::/10 Neighbor discovery and routing, primarily used by routers to discover links

## EUI-64
Unicast address, guaranteed uniqueness
inserts "FFFE" bits into host portion of address, driving part of the host address up a section
2001:AC:C0:A::1234:5678:9100/64
2001:AC:C0:A:1235:56FF:FE78:9100/64
123456 pushed up a space in host address, and the bit is increased by 1 to 1235

## Anycast
Used for router discovery

## Multicast
Sends to group of devices
FF00::/12

