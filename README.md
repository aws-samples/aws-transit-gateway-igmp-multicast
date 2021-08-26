## AWS Transit Gateway IGMP Multicast

The [AWS CloudFormation](http://aws.amazon.com/cloudformation/) template in this repository, [multicast.yaml](multicast.yaml), builds a simple architecture in AWS as shown in the diagram below. This can be used to demonstrate the operation of the [AWS Transit Gateway](http://aws.amazon.com/transit-gateway) multicast feature with IGMP, as [described on the AWS blog](https://aws.amazon.com/blogs/networking-and-content-delivery/automating-service-discovery-using-aws-transit-gateway-multicast-with-igmp/).

<img src="multicast-diag.png">

### Update 2021-08-26

CloudFormation now [documents](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ec2-transitgatewaymulticastdomain.html) the `igmpv2Support` option to the `AWS::EC2::TransitGatewayMulticastDomain` resource type. The template [multicast-v2.yaml](multicast-v2.yaml) uses this to automate completely the creation of the architecture. If you launch this version of the stack, you can skip ahead to the section [**Demonstrating multicast operation** in the blog](https://aws.amazon.com/blogs/networking-and-content-delivery/automating-service-discovery-using-aws-transit-gateway-multicast-with-igmp/).

## Security

As built by the template, no resources are publicly accessible from the internet or from any other VPC.

## Contributing

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

