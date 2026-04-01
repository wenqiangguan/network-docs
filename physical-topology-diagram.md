graph TD

    subgraph Entry_Area["Entry / Utility Closet"]
        Modem["ISP Modem"]
    end

    subgraph Living_Room["Living Room"]
        Router["WiFi Router"]
        Switch["5-Port Gigabit Switch"]
        TV["Smart TV"]
        Console["Game Console"]
        NAS["NAS (Optional)"]
    end

    subgraph Bedroom["Bedroom"]
        PC["Bedroom PC / Laptop Dock"]
    end

    %% Connections
    Modem -->|Ethernet| Router
    Router -->|LAN1| Switch
    Router -->|LAN2| NAS

    Switch --> TV
    Switch --> Console
    Switch --> NAS
    Switch -->|Ethernet Wall Jack| PC

    %% WiFi Devices
    Router -. WiFi .-> Phone["Smartphones / Tablets / Laptops"]
    Router -. WiFi .-> IoT["IoT Devices (Smart Speaker, Bulbs, etc.)"]
