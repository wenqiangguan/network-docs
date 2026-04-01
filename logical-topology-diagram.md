# Logical Topology Diagram

```mermaid
graph TD

Internet["Internet"]
Modem["ISP Modem (Bridge Mode)"]
Router["Home WiFi Router<br/>Gateway: 192.168.10.1<br/>DHCP + DNS Forwarding"]

subgraph LAN["LAN: 192.168.10.0/24"]
    Switch["Gigabit Switch"]
    NAS["NAS (192.168.10.10)"]
    TV["Smart TV (192.168.10.20)"]
    Console["Game Console (192.168.10.21)"]
    PC["Bedroom PC (192.168.10.30)"]

    WiFi["WiFi Network<br/>SSID: Home-Primary"]
    Guest["Guest WiFi<br/>SSID: Home-Guest<br/>Isolated"]
end

Internet --> Modem --> Router
Router --> Switch
Router --> WiFi
Router --> Guest

Switch --> NAS
Switch --> TV
Switch --> Console
Switch --> PC

WiFi --> Phone["Phones / Tablets / Laptops"]
WiFi --> IoT["IoT Devices"]
