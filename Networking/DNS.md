## DNS (Domain Name System)

DNS is like the **phonebook of the internet**.

- Converts **domain names** (example.com) into **IP addresses** (192.168.1.1)
- Without DNS, you would have to remember numbers instead of names
- Helps browsers, apps, and devices **find each other**

---

### How DNS Works (Step by Step)

1. You type a website URL in your browser
2. Your device asks the **local DNS resolver** (usually ISP)
3. Resolver checks if it already knows the IP
   - If yes → returns IP to your device
   - If no → queries **root DNS servers**
4. Root server points to **Top Level Domain (TLD) server** (.com, .org, etc.)
5. TLD server points to **Authoritative DNS server** for the domain
6. Authoritative server returns the **IP address**
7. Your device uses this IP to connect to the website

> Result: You see the website in your browser

---

## DORA (DHCP Process)

DORA = **Discover, Offer, Request, Acknowledge**  
Used by **DHCP (Dynamic Host Configuration Protocol)** to assign IP addresses automatically.

### Steps:

1. **Discover**  
   - Client sends a broadcast to find a DHCP server

2. **Offer**  
   - DHCP server replies with an **available IP address** and other network info

3. **Request**  
   - Client says “I accept this IP, please assign it to me”

4. **Acknowledge**  
   - DHCP server confirms assignment  
   - Client can now use the IP to communicate on the network

> Simple way to remember: **D → O → R → A** = “**Do Offer Right Assignment**”

---

### Quick Notes

- DNS = maps **names → IPs**
- DHCP/DORA = assigns **IPs automatically**
- Both are essential for **network communication**
