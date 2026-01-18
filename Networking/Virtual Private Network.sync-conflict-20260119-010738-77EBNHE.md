## Virtual Private Network(VPN)

> **ISP : Internet Service Provider**

It creates an **encrypted tunnel** between:

> Your device ←→ VPN server ←→ Internet

so ; 

- Your ISP can’t see what you visit
    
- Websites see VPN IP, not your real IP
    
- Traffic becomes private and secure

```

SSL : Secure Socket Layer 
SSL Inspection 
```



##  How VPN Actually Works

1. You connect to VPN app
    
2. App creates encrypted tunnel
    
3. All traffic goes to VPN server first
    
4. VPN server forwards to website
    
5. Reply comes back through tunnel


# VPN vs Proxy vs Tor – Short Notes

## Core Methods Used

- **VPN → Tunnel Method**
  - Creates encrypted tunnel between you and VPN server  
  - All traffic goes inside one protected pipe

- **Proxy → Forwarding Method**
  - Simply forwards your request through another IP  
  - No real encryption

- **Tor → Hop Method**
  - Traffic jumps through 3 random nodes  
  - Each node knows only next + previous hop

---

## How Traffic Flows

### VPN
You → 🔐 Tunnel → VPN Server → Website

### Proxy
You → Forward → Proxy → Website

### Tor
You → Hop1 → Hop2 → Hop3 → Website

---

## What Each Hides

### VPN hides
- Real IP from websites  
- Browsing from ISP  
- Data on public Wi-Fi

VPN provider can still see traffic.

### Proxy hides
- Only your IP  
- Does NOT hide data  
- ISP can still see everything

### Tor hides
- Your IP from site  
- Your browsing from ISP  
- Strong identity separation

---

## Comparison Table

| Feature | VPN | Proxy | Tor |
|---|---|---|---|
| Method | Tunnel | Forwarding | Hop |
| Encryption | Yes | Mostly No | Yes |
| Hide from ISP | Yes | No | Yes |
| Hide IP from site | Yes | Yes | Yes |
| Speed | Fast | Fast | Slow |
| Anonymity | Medium | Low | High |

---

## Why VPN + Proxy Reduces Privacy

VPN → Proxy → Website

Problems:
- Two companies can log you  
- Encryption ends at proxy  
- More leaks (DNS, headers)  
- Easier correlation of logs

> More middlemen = less anonymity

---

## Best Use Cases

- **VPN:** privacy, public Wi-Fi, streaming  
- **Proxy:** quick IP change, app specific  
- **Tor:** real anonymity, sensitive research

---

## Golden Line

- VPN = Privacy  
- Proxy = Convenience  
- Tor = Anonymity
