# Lost Packets 

## Computer Networks Project

A multi-machine Computer Networks project demonstrating networking concepts using four Mac machines connected over a private LAN.

---

## Team Members

| Member | Machine | IP Address | Role |
|---|---|---|---|
| **Riya Garg** | Mac 1 | `10.7.19.168` | Private DNS Server + Test Client |
| **Vanshika Yadav** | Mac 2 | `10.7.14.3` | Edge Reverse Proxy + Load Balancer |
| **Nitanshu Goyal** | Mac 3 | `10.7.6.33` | Backend Server A |
| **Krish Garg** | Mac 4 | `10.7.20.243` | Backend Server B + Test Client |

---

## Network Information

All four machines are connected to the same private LAN/Wi-Fi network.

| Configuration | Value |
|---|---|
| Network | Private LAN |
| Subnet Mask | `255.255.224.0` |
| Prefix | `/19` |
| Gateway | `10.7.0.1` |
| Active Interface | `en0` |

---

## Network Architecture

```text
                         Private LAN / Wi-Fi
                                │
        ┌───────────────────────┼───────────────────────┐
        │                       │                       │
        │                       │                       │
     Mac 1                   Mac 2                   Mac 3
     Riya                  Vanshika                Nitanshu
  10.7.19.168              10.7.14.3               10.7.6.33
  Private DNS            Nginx Edge              Backend A
    + Client           Reverse Proxy              Port 3001
                            │
                            │
                            └───────────────┐
                                            │
                                         Mac 4
                                         Krish
                                      10.7.20.243
                                      Backend B
                                      Port 3002
```

To do - how to run the backends 
