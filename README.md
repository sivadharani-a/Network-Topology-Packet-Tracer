
🚀 Basic Network Topology Design Using Cisco Packet Tracer


📚 Project Description

This project demonstrates the design and configuration of a simple computer network using **Cisco Packet Tracer**.  
It involves two PCs connected through switches and a router, enabling communication across two different subnets.

---

🛠 Devices Used

- 1 × Router (Cisco 1941 or 2911)
- 2 × Switches (Cisco 2960)
- 2 × PCs
- Copper Straight-Through Cables



🌐 Network Topology Diagram

```
 PC1 ---- Switch1 ----|
                      |---- Router ---- Switch2 ---- PC2
```


Configuration Steps

1. Router Configuration

bash
enable
configure terminal

interface GigabitEthernet0/0
ip address xxx.xxx.xxx.x.x xxx.xxx.xxx.x 
no shutdown
exit

interface GigabitEthernet0/1
ip address xxx.xxx.xxx.x.x xxx.xxx.xxx.x 
no shutdown
exit

end
write memory




2. PC Configuration

PC1:
- IP Address: `192.168.1.10`
- Subnet Mask: `255.255.255.0`
- Default Gateway: `192.168.1.1`

PC2:
- IP Address: `192.168.2.10`
- Subnet Mask: `255.255.255.0`
- Default Gateway: `192.168.2.1`

➡️ Set these via: Desktop tab → IP Configuration in Packet Tracer.



🧪 Verification

From PC1, open Command Prompt and run:
```bash
ping 192.168.2.10
```

✅ If the ping is successful, the configuration is correct and the devices are communicating across the network.



📁 Files Included

- `basic_network_topology.pkt` → Cisco Packet Tracer project file
- `README.md` → Project documentation



🌟 Learning Outcomes

- Basic understanding of LAN design
- Practical experience with Cisco Packet Tracer
- Router and PC interface configuration
- Network communication verification using ICMP (ping)



🚧 Future Enhancements

- Add a web server to simulate HTTP access
- Implement VLANs and Inter-VLAN Routing
- Expand the topology with dynamic routing protocols like RIP or OSPF



