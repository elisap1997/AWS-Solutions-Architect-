## Introduction

privately connect your vpc to other aws services

eliminates need for internet gateway, nat device, vpn connection, or aws direct connect
instances in vpc do not require public ip address
traffic btwn vpc and other services do not leave aws network
horizontally scaled
allows secure communication?
two types, interface and gateway

## Interface Endpoints

elastic network interfaces w private ip address
serve as entry point for traffic going to a supported service
powered by aws privatelink, access services hosted on aws easily and securely by keeping your network traffic within the aws network
supports a ton of aws services
is not free 7.5 usd a month? as of 2020????

## Gateway Endpoints

target for specific route in route table, used for traffic destined for supported aws service


free, currently ? only supposrts dynamodb and s3

to create, specify vpc which you want to create endpoint, and service to which you want to establish connection
