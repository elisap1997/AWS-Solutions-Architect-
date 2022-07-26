# VPC Follow Along

## Create VPC, IGW, Route Tables and Subnets 

notice the default vpc in your region
tenancy is a dedictaed host?, very expensive, keep default
internet gateways so that outside world can reach it
main route table is whichever will be used as a default
create private route table for private subnets

## Launch an EC2 Instance

create new iam role for access to s3
create new security group

## Groups, NACL and Bastion

can name instances after created
security groups by default can only allow rules, cannot create deny rules!
aws marketplace for bastion

## NAT

nat gateway creates gateway to internet
nat instance can be used if you want to save money
want to ping internet to update packages

## VPC Endpoints

access s3 via cli
endpoint can connect to s3 wout nat gateway

## Flow Logs

track all the traffic going through VPC
send to cloudwatch or s3 bucket
might need an iam role for this

## Cleanup

make sure to do this so you dont incur costs
delete instances
check everything!!!!!
double check gateways
