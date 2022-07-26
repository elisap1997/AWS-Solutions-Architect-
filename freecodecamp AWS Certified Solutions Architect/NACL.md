# NACL

Network Access Control List Introduction

optional layer of security, acts as a firewall for controll traffic in and out of subnet

vpcs automatically get nacl

each nacl contains set of rules that can allow or deny traffic into inbound and outbound subnets

rule # determines order of evaluation, highest to lowest, highest # can be 32766 recommended to work in 10 or 100 increments

can allow or deny traffic, could block single ip address (cant do this w security groups)

## Use Case

determine malicious actor w specific ip address, trying to access our instance

block their ip

dont need to ssh into instances, just add a deny to the subnets

do this just in case our security groups ssh port was left open

security groups cannot deny single ip address

