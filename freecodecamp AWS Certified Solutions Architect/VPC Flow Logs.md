## VPC Flow Logs

allow you to capture ip traffic info in and out of network interface within vpc

can be created for vpc, subnets, network itnerface

all log data stored w amazon cloudwatch logs

after created, can be viewed in detail within cloudwatch logs

can send to s3 bucket

## Log Breakdown

stores source ip address and destination ip address

contains ip addresses not hostnames!!!!

some instance traffic not moniroted
* instance traffic generated b contacting aws dns servers
* windows license activation traffic from instances
* traffic to and from the instance metadata address
* dhcp traffic
* any traffic to reserved ip address of default vpc router
