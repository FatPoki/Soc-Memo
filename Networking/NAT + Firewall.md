## NAT (Network Address Translation)

NAT is used to **convert private IP addresses to public IP addresses** so devices inside a network can communicate with the internet.

---

### How NAT Works (Simple Steps)

1. Device in private network sends a request to the internet  
   - Example: PC with **IP 192.168.1.5** wants to visit `example.com`

2. NAT device (usually a router) **replaces the private IP** with its **public IP**  
   - Public IP: `103.45.67.89`

3. Router keeps a **translation table** to know which response belongs to which device

4. Response from internet comes to public IP → NAT router looks up the table → sends it to **correct private IP**

---

### NAT Example

| Private IP      | Public IP       |
|-----------------|----------------|
| 192.168.1.5     | 103.45.67.89   |
| 192.168.1.6     | 103.45.67.89   |

> Multiple devices can use **same public IP** with NAT using **different port numbers** (PAT / Port Address Translation).

---

## Firewall

A firewall is a **security barrier** between your internal network and the internet.  
It **monitors and controls network traffic** based on rules.

---

### How Firewall Works (Step by Step)

1. Device sends or receives data packets
2. Firewall inspects packets (IP, port, protocol, content)
3. Firewall applies rules:
   - **Allow** trusted traffic
   - **Block** untrusted traffic
4. Only approved traffic passes → network stays protected

---

### Types of Firewalls

| Type                 | Description (Easy)                                         |
| -------------------- | ---------------------------------------------------------- |
| **Packet Filtering** | Checks **IP, port, protocol**; fast but simple             |
| **Stateful**         | Tracks **connection state**; smarter than packet filtering |
| **Proxy Firewall**   | Acts as **middleman** between client and server            |
| **Next-Gen (NGFW)**  | Combines firewall + antivirus + IDS/IPS                    |
___

### Quick Summary

- NAT = **Private → Public IP translation**  
- Firewall = **Monitors traffic and blocks threats**  
- NAT + Firewall together = **Secure internet access for multiple devices**