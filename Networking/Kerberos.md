## Kerberos 

Kerberos is an **authentication system** that proves who you are **without sending your password again and again** on the network.

### Why Kerberos is needed
- Sending passwords over a network is **unsafe**
- Attackers can capture passwords
- Kerberos avoids this by using **tickets instead of passwords**

### How Kerberos works (simple)
- User logs in **once**
- Kerberos verifies the user
- A **ticket** is issued
- User shows this ticket to different services
- Services trust the ticket and allow access

### Why tickets are safer
- Password is **never sent** after login
- Tickets have a **time limit**
- Expired tickets cannot be reused

### Single Sign-On (SSO)
- Login **one time**
- Access **multiple services**
- No repeated login prompts

### Where Kerberos is used
- Company networks
- Windows Active Directory
- Universities and cloud systems

> **One-line memory tip:**  
> Kerberos = *Login once, use tickets, no password sharing*