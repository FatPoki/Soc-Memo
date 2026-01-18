

> [!info] Transmission Control Protocol / Internet Protocol
> - A **5-layer model**
> - Acts mostly like the **OSI model**
> - Some OSI layers are **combined**

---

## TCP/IP Layers

> [!note] Layer 5 – Application
> - Consists of **applications & processes** that use the network

> [!abstract] Layer 4 – Transport
> - Provides **end-to-end data delivery service**

> [!example] Layer 3 – Network
> - Performs **logical addressing**
> - Handles **routing of data packets**

> [!example] Layer 2 – Data Link
> - Combines raw data into **frames**
> - Performs **error recovery & retransmission**
> - **MAC address** is identified here

> [!example] Layer 1 – Physical
> - Provides **physical interface**
> - Responsible for **data transmission**

---

## My Summary

> [!summary]
> - User sends request from the **Application layer**
> - Through the **Transport layer**, a connection is made with the destination
> - In the **Network layer**, **source IP & destination IP** are extracted
> - In the **Data Link layer**, **error recovery** is done and data is converted into **frames**
> - **MAC address** is identified at this layer
 

# TCP vs UDP

> [!note] TCP (Transmission Control Protocol)
> - **Connection-oriented** protocol  
> - Uses **3-way handshake** (SYN, SYN-ACK, ACK)  
> - **Reliable** data transfer  
> - Slower than UDP  
> - Used where **accuracy matters** (web, email, file transfer)

> [!example] UDP (User Datagram Protocol)
 >
> - **Connection-less** protocol  
> - **No handshake**  
> - **Non-reliable** data transfer  
> - **Real-time** and faster  
> - Used where **speed matters** (video streaming, gaming, VoIP)