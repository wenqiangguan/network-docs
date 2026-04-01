# Logical Topology – 1B1B Apartment Network

## 1. Network Structure
- **Topology Type:** Star topology
- **Core Device:** Home WiFi Router
- **Upstream:** Router WAN → ISP Modem → Internet
- **Downstream:**
  - Wired: Switch, NAS, Smart TV, Game Console, Bedroom PC
  - Wireless: Phones, laptops, tablets, IoT devices

## 2. Subnet and Addressing
- **Primary LAN Subnet:** 192.168.10.0/24
- **Default Gateway:** 192.168.10.1
- **DHCP Range:** 192.168.10.100–192.168.10.199
- **Static IP Range:** 192.168.10.2–192.168.10.50

## 3. VLAN Design (Optional)
- VLAN 10 – Main devices (PC, NAS)
- VLAN 20 – IoT devices
- VLAN 30 – Guest WiFi

> VLANs are not currently deployed but reserved for future expansion.

## 4. Logical Relationships
- Router provides NAT, DHCP, DNS forwarding
- All devices use 192.168.10.1 as gateway
- NAS provides file sharing and media services

## 5. Wireless Network Logic
- **Primary SSID:** Home-Primary  
  For personal devices  
- **Guest SSID:** Home-Guest  
  Isolated from internal network

