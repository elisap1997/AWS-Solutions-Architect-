# VPC

provision logically isolated section of aws clous can launch aws resources in virtual network you define

## core componenets

think of it as personald ata cneter
gives you complete control over your virtual networking envrionment

this is in every aws cert bar cloud practioner!

Core components:

internet gateway, virtual private gateway, routing tables, network access control lists -stateless, security groups stateful, public subnets, private subnets, nat gateway, customer gateway, vpc endpoints, vpc peering

## key features

are region specific, can create 5 per region, each region comes with default one, can have 200 subnets per vpc, can use ipv4 cidr block and in addition to ipv6 cidr blocks (the address of the vpc), cost nothing (vpcs, route tables, nacls, intenret gateways, security groups and subnets, vpc peering), price (nat gateway, vpc endpoints, vpn gateway, customer gateway), dns hostnames if instance have domain name addresses

## default vpc

can immediately launch instances

creates vpc w size 16 ipv4 cidr block 172.31.0.0/16
creates size /20 default subenet in each availlabilit zone
creates itnert gateway and connect it to default vpc
creates default security group and associate it w default vpc
creates default network access control list (NACL) and associate it with your default vpc
associate the default dhcp options set for your aws account with your default vpc
associate the default dhcp options set for your aws account with your default vpc
when create vpc automaticall has a main route table

## default everywhere ip

0.0.0.0/0 is default

represents all possible ip addresses

just think of giving access from anywhere from the internet

## vpc peering

allows you to connect one vpc with another over a direct network route using private ip addresses

instances on peered vpcs behave like on same network

can connect vpcs across same or diff aws accounts and regions

peering uses star config: 1central vpc-4 other vpcs

no transitive peering, peering mus ttake place directly btwn vpcs, one-to-one

cant have overlapping cidr blocks

## route tables

determine where network traffic direct

each subnet in vpc must be associated w route table

subnet onl associate w one route table at time, but can associate multiple subnets with same route table

allowing ec2 instances to gain access to the internet

## internet gateway

allows your vpc access to internet

does two things:
1. provide tagert in vpc route tables for internet-routable traffic
2. perform network address translation (NAT) for instances that ahve been assigned public ipv4 addresses

to route out to internet need to add in route tables need to add a route to the internet gatewa and set destination to default everywhere ip
