# OSI model 

> [!info] OSI (Open System Interconnection)
> - OSI is a **7-layer theoretical reference model**
> - Developed by **ISO**
> - A **universal standard** for networking & communication
> - **All layers are strictly independent**

---

## OSI Model

### Host Layers

> [!note] Layer 7 – Application
> **Data:** Data  
> **Function:** Network process to application

> [!note] Layer 6 – Presentation
> **Data:** Data  
> **Function:** Recognising / formatting data

> [!note] Layer 5 – Session
> **Data:** Data  
> **Function:** Session establishment & termination

---

### Transport Layer

> [!abstract] Layer 4 – Transport
> **Data:** Segment  
> **Function:** End-to-end connectivity & reliability

---

### Media Layers

> [!example] Layer 3 – Network
> **Data:** Packets  
> **Function:** Logical addressing & path determination

> [!example] Layer 2 – Data Link
> **Data:** Frames  
> **Function:** Physical addressing

> [!example] Layer 1 – Physical
> **Data:** Bits  
> **Function:** Media signals & binary transmission

---

## My Summary

> - Host sends data from **Layer 1 → Layer 2**, where **physical addressing** is done  
> - In **Layer 3 & 4**, **IP and destination** are extracted and a **connection** is made  
> - **Client session** is established  
> - Data is **encapsulated in presentable format**  
> - Finally sent to **Layer 7 (Application layer)**