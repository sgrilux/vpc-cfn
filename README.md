# VPC - Cloudformation

Generic Two tiers (public-private) VPC in 3 AZ.

## Parameters

- **VpcName**: Name of the VPC [default: dev]
- **VpcCidr**: CIDR [default: 10.0.0.0/16]
- **PublicSubnet1Cidr**: Public Subnet AZ A [default: 10.0.0.0/24]
- **PublicSubnet2Cidr**: Public Subnet AZ B [default: 10.0.1.0/24]
- **PublicSubnet3Cidr**: Public Subnet AZ C [default: 10.0.2.0/24]
- **PrivateSubnet1Cidr**: Public Subnet AZ A [default: 10.0.3.0/24]
- **PrivateSubnet2Cidr**: Public Subnet AZ B [default: 10.0.4.0/24]
- **PrivateSubnet3Cidr**: Public Subnet AZ C [default: 10.0.5.0/24]
- **VpcFlowLogs**: Enable VPC FlowLogs [default: false]

## Outputs

- **VpcId**: [export: '${AWS::StackName}::vpc-id' ]
- **PublicSubnet1**: [export: '${AWS::StackName}::public-subnet-id-1']:
- **PublicSubnet2**: [export: '${AWS::StackName}::public-subnet-id-2']
- **PublicSubnet3**: [export: '${AWS::StackName}::public-subnet-id-3']
- **PrivateSubnet1**: [export: '${AWS::StackName}::private-subnet-id-1']
- **PrivateSubnet2**: [export: '${AWS::StackName}::private-subnet-id-2']
- **PrivateSubnet3**: [export: '${AWS::StackName}::private-subnet-id-3']
