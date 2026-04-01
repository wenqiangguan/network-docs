# Device Configurations – 1B1B Apartment Network (Example)

> Note: No real passwords are included. Only structure and configuration concepts are shown.

## 1. Router Configuration

### WAN
- Connection type: DHCP (ISP assigned)
- DNS override: 1.1.1.1 / 8.8.8.8

### LAN
- IP: 192.168.10.1
- Mask: 255.255.255.0

### DHCP
- Range: 192.168.10.100–199
- Reservations:
  - NAS → 192.168.10.10
  - TV → 192.168.10.20
  - Console → 192.168.10.21
  - PC → 192.168.10.30

## 2. WiFi Configuration

### Primary SSID
- Name: Home-Primary
- Security: WPA2/WPA3-Personal
- Password stored in password manager

### Guest SSID
- Name: Home-Guest
- Client isolation enabled
- No access to internal LAN

## 3. Port Forwarding (Example)
- Game Console:
  - External Port: 3074
  - Internal IP: 192.168.10.21
  - Protocol: TCP/UDP

## 4. Firewall Rules
- LAN → WAN: Allow
- WAN → LAN: Deny (except established connections)
- Guest network blocked from 192.168.10.0/24
- IoT devices restricted from accessing NAS/PC

