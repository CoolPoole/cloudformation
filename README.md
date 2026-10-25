# Welcome to CloudFormation

Repos designated to CloudFormation labbing and learning

## Notes

The notes folder contains individual notes around the learned aspect of Cloudformation.

Contents:
---
- Parameters
- Resources
- Mappings
- Conditions
- Outputs
- Rules
- Metadata

## Files

### securitygroup.yaml
---

- Contains parameters, resources, and outputs to show AWS EC2 Security Group creation
- Uses !Sub, !Ref commands
- Type:
    - AWS::EC2::SecurityGroup

### vpc.yaml
---

- Contains parameters, metadata, resouces, and outputs to show creation of VPC, Subnets, Internet Gateway, and Route Tables
- Uses !Ref, !Sub, !Select, !GetAZs commands
    - !Ref is used to reference resouces
    - !Sub is to substitue a parameter value into a string
    - !Select is to grab a value out of an array
    - !GetAZs grabs the list of AZs and puts them into an array
- Types:
    - AWS::EC2::VPC
    - AWS::EC2::InternetGateway
    - AWS::EC2::VPCGatewayAttachment
    - AWS::EC2::Subnet
    - AWS::EC2::RouteTable
    - AWS::EC2::Route
    - AWS::EC2::SubnetRouteTableAssociation





