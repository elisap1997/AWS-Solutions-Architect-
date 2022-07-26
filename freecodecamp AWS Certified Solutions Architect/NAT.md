# NAT

Network Address Translation

method of re-mapping one IP address space to another

use NAT gateways to remap private IPs
  - if you have private network and need help to gain outbound access to the internet

use NAT to make addresses more agreeable
  - if you have two networks which have conflicting network addresses

## NAT instances vs NAT gateways

must run within public subset

instances - (legacy)
  - individual EC2 instances
  - community AMIs exist to launch NAT instances

gateways
  - managed ervice
  - launches redundant instances within selected AZ
