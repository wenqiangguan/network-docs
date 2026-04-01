# Physical Topology – 1B1B Apartment Network

## 1. Apartment Layout Overview
This documentation is based on a typical 1 Bedroom / 1 Bathroom apartment.  
Main areas include:
- Entry / Utility Closet
- Living Room
- Bedroom
- Kitchen
- Bathroom

## 2. Physical Device Locations

### ISP Modem
- **Location:** Entry area or utility closet
- **Connection:** ISP line → Modem WAN

### Main WiFi Router
- **Location:** Living room TV stand
- **Connections:**
  - WAN → Modem LAN
  - LAN1 → Switch
  - LAN2 → NAS (optional)
- **Wireless Coverage:** Living room, kitchen, partial bedroom

### Switch (5‑port Gigabit, optional)
- **Location:** Living room TV stand
- **Connections:**
  - Port 1 → Router LAN1
  - Port 2 → Smart TV
  - Port 3 → Game Console
  - Port 4 → Bedroom wall Ethernet jack
  - Port 5 → NAS (if not directly connected to router)

### Bedroom Devices
- Wall Ethernet jack → PC / Laptop Dock  
- WiFi for mobile devices

### Wireless Devices
- Smartphones, tablets, laptops
- Smart speakers
- Smart bulbs, plugs, IoT devices

## 3. Physical Connection Diagram (Text Version)

- ISP → Modem  
- Modem LAN → Router WAN  
- Router LAN → Switch  
- Switch → TV / Console / NAS / Bedroom Ethernet  
- Bedroom Ethernet → PC  

## 4. Topology Diagram
A diagram file should be included as **physical-topology.png**, showing:
- Device names
- Room locations
- Wired vs wireless links
- Interface labels (WAN, LAN1, Port1, etc.)

