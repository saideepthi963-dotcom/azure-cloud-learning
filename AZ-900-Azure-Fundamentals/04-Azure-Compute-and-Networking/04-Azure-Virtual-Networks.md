# Azure Virtual Networks (VNets)

## 1. What Is an Azure Virtual Network?

An **Azure Virtual Network (VNet)** is a private network in Azure that allows cloud resources, such as Virtual Machines, to communicate securely.

Think of it as creating your own private network inside Azure, where you control which resources can communicate and how traffic flows.

## 2. VNets, Subnets, and IP Addresses

When creating a VNet, you first choose an **IP address range** (address space), such as `10.0.0.0/16`.

You can then divide this network into smaller networks called **subnets**.

For example:

```text
Azure Virtual Network (10.0.0.0/16)
          │
          ├── Subnet 1: Web Application
          │       └── VM 1
          │
          └── Subnet 2: Database
                  └── VM 2
```

**VNet →** Your private Azure network.

**Subnet →** A smaller section within your VNet.

**IP Address →** Identifies a resource on the network.

**NIC (Network Interface Card) →** Connects a resource, such as a VM, to the VNet.

Resources within the same VNet can communicate privately by default, although security rules can restrict communication.

## 3. Connecting Azure Networks

Imagine a company has resources in multiple Azure networks and also owns an on-premises datacenter.

Azure provides different connectivity options:

| Service | What It Does |
|---|---|
| **VNet Peering** | Connects two Azure VNets through Microsoft's private network. |
| **VPN Gateway** | Connects networks through encrypted tunnels over the internet. |
| **Azure ExpressRoute** | Provides private connectivity to Microsoft cloud services through a connectivity provider. |

**Remember:**

**VNet Peering →** Connect Azure VNets.

**VPN Gateway →** Encrypted connection over the internet.

**ExpressRoute →** Private connectivity that doesn't use the public internet for the connection.

## 4. Routing in Azure VNets

**Routing** determines where network traffic travels.

Azure automatically creates system routes, so basic network communication works without manually configuring routes.

If you want to control the path traffic takes, you can create **User-Defined Routes (UDRs)**.

For example, you can direct traffic through a firewall for additional inspection.

## 5. Network Security Groups (NSGs)

A **Network Security Group (NSG)** controls incoming and outgoing network traffic using security rules.

Imagine you have a database VM that should only accept connections from your application's subnet.

An NSG can help restrict access using rules based on IP addresses, ports, and protocols.

NSGs can be associated with **subnets** or **network interfaces (NICs)**.

**Remember:** NSG = Allow or deny network traffic.

## 6. Private Endpoints

A **Private Endpoint** allows supported Azure services, such as Azure Storage or Azure SQL Database, to be accessed through a private IP address inside your VNet.

Instead of accessing the service through its public endpoint, your resources can communicate privately using Azure networking.

**Remember:** Private Endpoint = Private access to an Azure service.

## 7. Good VNet Design Practices

Keep network address ranges from overlapping when networks need to connect.

Use separate subnets for different workloads, such as web applications and databases. This makes it easier to apply specific security rules.

Monitor network routes and traffic to understand how resources communicate.

---

## ⭐ Important AZ-900 Concepts

| Concept | Simple Meaning |
|---|---|
| **VNet** | Private network in Azure |
| **Subnet** | Smaller network inside a VNet |
| **NIC** | Connects a VM or other supported resource to a network |
| **VNet Peering** | Connects Azure VNets |
| **VPN Gateway** | Encrypted network connection over the internet |
| **ExpressRoute** | Private connectivity to Microsoft cloud services |
| **UDR** | Custom network routing |
| **NSG** | Controls inbound and outbound traffic |
| **Private Endpoint** | Private access to supported Azure services |

### Main Takeaway

Azure Virtual Networks provide the foundation for **private communication, network connectivity, routing, and security** in Azure.