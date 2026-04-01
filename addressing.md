# Addressing Documentation – 1B1B Apartment Network

## 1. Network Information
- **Subnet:** 192.168.10.0/24
- **Gateway:** 192.168.10.1
- **Subnet Mask:** 255.255.255.0
- **DNS Servers:**
  - Primary: 1.1.1.1
  - Secondary: 8.8.8.8

## 2. DHCP Pool
- **Range:** 192.168.10.100–192.168.10.199
- **Lease Time:** 24 hours

## 3. Static IP Assignments

| Device        | Role/Use            | IP Address      | MAC Address | Location | Notes |
|---------------|----------------------|------------------|-------------|----------|-------|
| Router        | Gateway/DHCP/DNS     | 192.168.10.1     | AA:AA:AA... | Living Room | LAN interface |
| NAS           | Storage/Media        | 192.168.10.10    | BB:BB:BB... | Living Room | Static IP |
| Smart TV      | Streaming            | 192.168.10.20    | CC:CC:CC... | Living Room | DHCP reservation |
| Game Console  | Gaming               | 192.168.10.21    | DD:DD:DD... | Living Room | Port forwarding |
| Bedroom PC    | Work/Entertainment   | 192.168.10.30    | EE:EE:EE... | Bedroom | Wired |

## 4. DHCP Devices (Examples)

| Device       | Connection | IP Range Example        | Notes |
|--------------|------------|--------------------------|-------|
| Smartphone   | WiFi       | 192.168.10.100–120       | DHCP |
| Laptop       | WiFi       | 192.168.10.121–140       | DHCP |
| Tablet       | WiFi       | 192.168.10.141–160       | DHCP |
| Smart Speaker| WiFi       | 192.168.10.161–180       | DHCP |

