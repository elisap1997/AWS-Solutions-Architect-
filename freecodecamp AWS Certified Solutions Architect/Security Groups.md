# Security Groups

virtual firewall that controls traffic to and from ec2 instances
associate w ec2 instances
provide security at protocol and port access level
contains set of rules that filter traffic coming into inbound and outbound ec2 instances
all traffic blocked by default unless a rule specifically allows it
multiple instances across multiple subnets can belong to security group

## Use Cases

specify source to be an ip range or specific ip
can specify source to be another security group
instance can belong to multiple security groups and rules are permissive
  - if you have one security group which has no allow and you ass an allow to another than it will allow

## Limits

upto 10000 security groups in a region (default 2500)
60 inbound and 60 outbound rules per security group
16 security groups per elastic network interface (ENI) (default is 5)
