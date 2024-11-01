# Networking in Amazon EC2<a name="ec2-networking"></a>

* Amazon VPC
  * enables you to
    * ⭐️launch AWS resources (_Example:_ Amazon EC2 instances) | it(VPC) | your AWS account ⭐️
      * when you launch the instance -> you can select a subnet | VPC
      * -- configured with a -- primary network interface
        * 👀== logical virtual network card 👀 
        * -> the instance -- receives a -- primary private IP address /
          * from the subnet's IPv4 address
          * -- assigned to the -- primary network interface
      * 👀you can control whether the instance -- receives a -- public IP address / 👀
        * from Amazon's pool of public IP addresses
        * -- is associated with -- your instance ONLY UNTIL it is stopped or terminated
          * if you require a persistent public IP address -> allocate an Elastic IP address /
            * -- for -- your AWS account /
              * 👀remains associated with it UNTIL, you release it 👀
            * -- associate it with an -- 
              * instance or
                * Elastic IP address -- can be associated to another -- instance
              * network interface
      * possible to bring your own IP address range -- to -- your  AWS account

* ways to
  * increase network performance & reduce latency
    * launch instances | placement group
    * use enhanced networking
      * -> higher packet per second \(PPS\) performance
  * accelerate high performance computing & machine learning applications
    * usw an Elastic Fabric Adapter \(EFA\)
      * == network device / you can attach | supported instance type

**Topics**
+ [Regions and Zones](using-regions-availability-zones.md)
+ [Instance IP addressing](using-instance-addressing.md)
+ [Instance hostname types](ec2-instance-naming.md)
+ [Bring your own IP addresses](ec2-byoip.md)
+ [Assigning prefixes](ec2-prefix-eni.md)
+ [Elastic IP addresses](elastic-ip-addresses-eip.md)
+ [Network interfaces](using-eni.md)
+ [Network bandwidth](ec2-instance-network-bandwidth.md)
+ [Enhanced networking](enhanced-networking.md)
+ [Elastic Fabric Adapter](efa.md)
+ [Placement groups](placement-groups.md)
+ [Network MTU](network_mtu.md)
+ [Virtual private clouds](using-vpc.md)
+ [EC2\-Classic](ec2-classic-platform.md)