## What is cloud?
"The cloud" means a servers which is accessed over the Internet, and the software and databases or ther process that run on those servers. Cloud servers are located in data centers all over the world.

cloud details: [cloud](https://www.cloudflare.com/en-gb/learning/cloud/what-is-the-cloud/)
![ cloud ](./docs/images/cloud.png)

## Openstack
Openstack [Openstack](https://docs.openstack.org/install-guide/get-started-logical-architecture.html)


## What is virtualization?
Virtualization is technique that created multiple physical layer over single physical layer that can be used by multiple physical machine or sharing the resource.

Virtualization Details [virtualization](https://www.ibm.com/cloud/learn/virtualization-a-complete-guide)

![ virtualization ](./docs/images/virtualization.png)

## How virtualization work?

Physical layer() have some major component.Those ase  
        - application : when run application in usernamespace it's call different OS API.The OS api called System api.Application run always run usernamespace.   
        - os: make connection between application and karnel.  
        - karnel: manage the resource.  

how execution processor:   
    - fetch : is the operation which receives instructions from program memory from a systems RAM.   
    - Decode: the instruction is converted to understand which other parts of the CPU are needed to continue the operation. This is performed by the instruction decoder  
    - Execute: perfomr the operation and keep that Each part of the CPU that is needed is activated to carry out the instructions.  

Work flow: application->os->karnel  

![ virtualization works fllow ](./docs/images/vm-works.png)
![ virtualization works fllow ](./docs/images/work-flow-1.png)

## KVM 
KVM (for Kernel-based Virtual Machine) is a full virtualization solution for Linux on x86 hardware containing virtualization extensions (Intel VT or AMD-V). It consists of a loadable kernel module, kvm.ko, that provides the core virtualization infrastructure and a processor specific module, kvm-intel.ko or kvm-amd.ko.

[KVM link 1](https://www.linux-kvm.org/page/Main_Page)  
[KVM link 2](https://www.redhat.com/en/topics/virtualization/what-is-KVM)  


## Openvswitch:
Open vSwitch is a multilayer software switch licensed under the open source Apache 2 license. Our goal is to implement a production quality switch platform that supports standard management interfaces and opens the forwarding functions to programmatic extension and control.

[ Openvswitch ](https://docs.openvswitch.org/en/latest/intro/what-is-ovs/#overview)

![ Openvswitch ](./docs/images/open-v-switch.png)


## Linux bridge
linux bridge: Linux bridge behaves like a network switch. it's connect multiple vm in same network.
Every VM is connect to hub by veth(virtual Ethernet).

Linux bridge details: [ Linux bridge ](https://www.ibm.com/docs/en/linux-on-systems?topic=choices-using-linux-bridge)  
veth detail here: [veth](https://man7.org/linux/man-pages/man4/veth.4.html)

![ Linux bridge ](./docs/images/vm-img1.png)


## Domain collision?
The collision domain defines the set of devices on which their frames could collide. It is a network segment connected by a shared medium or using repeaters where real-time data transmissions collide.

[Domain collision](https://www.geeksforgeeks.org/collision-domain-and-broadcast-domain-in-computer-network/)


## VXLAN
VXLAN is an encapsulation protocol that provides data center connectivity using tunneling to stretch Layer 2 connections over an underlying Layer 3 network.

Details VXLAN: [VXLAN link 1](https://www.juniper.net/us/en/research-topics/what-is-vxlan.html), [VXLAN link 2](https://datatracker.ietf.org/doc/html/rfc7348)


![ vxlan-img-1 ](./docs/images/vxlan-img-1.png)

![ vxlan-img-2 ](./docs/images/vxlan-img-2.png)

![ vxlan-img-3 ](./docs/images/vxlan-img-3.png)


## DNAT(Destination network address translation)  

Destination network address translation(DNAT) is technique for frequently changing the destination ip address over end route packet and performing the inverse function for any replies or responce.The translation can be from a public IP address to a private IP address or vice versa.

Control flow: internet/server(10.10.10.1) -> media(DNAT) -> local or host machine(192.168.0.1)

## SNAT(Source network address translation)

Source Network Address Translation(SNAT) is technique that allows users in private network to access internet.SNAT rule will translate the inter ip address(private ip address) to public ip address.so that private network users can have access to public network via the public interface.

Control flow: internet/server(10.10.10.1 public) <- media(SNAT) <- local or host machine(private network192.168.0.1)

There 3 type os SNAT,
  - DIPP(Dynamic ip and port)
  - Dynamic IP
  - Static IP

![ SNAT ](./docs/images/snat.png)


## SDN(Software define network)

Software-Defined Networking (SDN) is an approach to networked that uses the software based controller or application programming interfaces (APIs) to communicate with underlying hardware infrastructure and direct traffic on a network.

[SDN](https://www.vmware.com/topics/glossary/content/software-defined-networking)

## Autonomous system

An autonomous system(as) is a collection of one or more associated connected internet protocol routing prefix under the control of one more netwrok operators on behalf on single entity or organization.

## ASN (Autonomous system Number)

Autonomous system is assigned a number that number is called ASN(Autonomous system Number). The number could be 16 or 32 bit numbers.There is a limited amount of ASNs available.

[AS](https://www.cloudflare.com/en-gb/learning/network-layer/what-is-an-autonomous-system/)

## Underlay Network

Underlay Network is physical infrastructure above overlay network is built. Underlying network responsible for delivery of packets across networks.


## Overlay Network

An Overlay Network is a virtual network which is built on top of underlying network (Underlay Network infrastructure). In other words, “Underlay or “Underlay network” provides a “service” to the overlay.













