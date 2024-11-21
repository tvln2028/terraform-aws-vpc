# Custom AWS VPC Module

![alt text](images/vpc.jpg)

This module is developed for joindevops.com


* VPC
* Internet Gateway
* Internet and VPC attachment
* 2 public Subnets
* 2 private Subnets
* 2 Database subnets
* EIP
* NAT GAteway
* public Route table
* private route table
* database route table
* Route table associations
* Routes in all tables
* peering if required for user
* Routes of peering in requestor and acceptor VPC
* Database subnet group


### INPUTS ####

* project_name (required): User should mention their project name. Type is string.
* environment (optional): Default value is true. Type is bool.
* common_tags (required): User should provide their tags related to their project. Type is map.
* vpc_cidr (optional): Default value is 10.0.0.0/16. Type is string.
* enable_dns_hostnames (optional): Default value is true. Type is bool.
* vpc_tags (optional): Default value is empty. Type is map.
* igw_tags (optional): Default value is empty. Type is map.
* public_subnet_cidrs (required): user has to provide 2 valid subnet CIDR.
* public_subnet_cidr_tags (optional): Default value is empty. Type is map.
* private_subnet_cidrs (required): user has to provide 2 valid subnet CIDR.
* private_subnet_cidr_tags(optional): Default value is empty. Type is map.
* database_subnet_cidrs (required): user has to provide 2 valid subnet CIDR.
* database_subnet_cidr_tags (optional): default value is empty. type is map.
* database_subnet_group_tags (optional): default value is empty. type is map.
* nat_gateway_tags (optional): default value is empty. type is map.
* public_route_table_tags (optional): default value is empty. type is map.
* private_route_table_tags (optional): default value is empty. type is map.
* database_route_table_tags (optional): default value is empty. type is map.
* is_peering_required (optional): default value is false. Type is bool.
* acceptor_vpc_id (optional): Default value is empty, default VPC ID would be taken. Type is string.
* vpc_peering_tags (optional): Default value is empty. Type is map.