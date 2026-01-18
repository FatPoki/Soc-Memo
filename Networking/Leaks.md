## VPN / Proxy / Tor Leaks

### 1) VPN Leaks
**What it tells:** Your real network info is escaping outside the VPN tunnel.

**Can leak:**
- Real IP address (IPv4/IPv6)
- DNS queries going to your ISP
- WebRTC revealing local IP

**VPN normally hides:**
- Public IP
- Location
- ISP identity
- Browsing traffic from ISP

**But NOT hide:**
- Accounts you log into  
- Cookies  
- Device fingerprint

---

### 2) Proxy Leaks
**What it tells:** The browser/app is bypassing the proxy and connecting directly.

**Can leak:**
- Real IP  
- DNS requests  
- Non-proxied apps/ports

**Proxy normally hides:**
- IP for specific app/browser only

**But NOT hide:**
- System traffic  
- Encryption  
- Identity inside sites

---

### 3) Tor Leaks
**What it tells:** Something is breaking Tor anonymity model.

**Can leak:**
- Real IP via WebRTC or plugins  
- DNS outside Tor  
- Login identity linking you

**Tor normally hides:**
- IP  
- Location  
- Browsing path  
- ISP from knowing visited sites

**But NOT hide:**
- Who you are if you log into personal accounts  
- Identity via plugins or browser changes

---

## Simple Comparison

| Technology | Hides | Can Leak |
|------------|-------|---------|
| VPN | IP, location, ISP spying | DNS, WebRTC, IPv6, app bypass |
| Proxy | IP for one app | System traffic, DNS, real IP |
| Tor | IP + routing anonymity | Browser plugins, logins, DNS |

---

### One-line takeaway
- **VPN leak = tunnel broken**  
- **Proxy leak = traffic bypassing proxy**  
- **Tor leak = anonymity chain exposed**

---

### Golden Rule
**Leak = failure of what the tool promises to hide,  
not exposure of things it was never designed to hide.**
