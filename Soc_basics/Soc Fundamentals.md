

### CIA traits
The CIA Triad is the foundational model used to guide security policies and protect an organization's assets.
The **CIA Triad** defines **what security is trying to protect**.

1. **Confidentiality**  : ensure the data is accessed by only authorized user
examples include encryption , access controls and classification.

2. **Integrity ** :  Ensure that data shared is consistant accurate and has not been tampered, to make this happen we use techniques like hashing, digital signature and checksums.

3.  **Availability :**  Ensure system data is available to access from anywhere and any time to authorised parties.

---

### Malware

Malware is any software that is designed with an intention to harm a system.

#### Type of malwares

1.  **virus** : Malicious code that attaches to files and spreads when opened.
   
2.  **worm** :  worms are program that replicate and spread across a network independently without any need to attach with any file unlike virus.
   
3. **Trojan horse** : trojan pretent like a normal software but once inside system the create a backdoor for the attacker.
   
4. **spyware** : spyware secretly monitors users activity and captures keystrokes browsing data habits and personal information.
   
5. **ransomware**: ransomware is a type of malware that encrypts the system files and locks them in demand for ransom.
   
6. **adware** : displays unwanted ads in user system in form of popups.
   
7. **root kit** :  root kits are highly stealthy they perform and gain root/admin access on system and hide whole on-going process of other malwares that are helping an attacker.

---
### MITRE ATT&CK

MITRE ATT&CK is a globally accessible knowledge base that documents **adversary tactics, techniques, and procedures (TTPs)** based on real-world cyberattack observations.

---


###  INCIDENT RESPONSE LIFECYCLE

The incident response lifecycle shows **how a SOC handles security incidents from start to finish**.

> **Phase**
> 1. Preparation
> 2. Identification
> 3. Containment
> 4. Eradication
> 5. Recovery
> 6. post incident activity


---


### Prepration

We make preparations for the breach so we can handle the situation when the time comes.
we can , create a plan , build the team , set up tools  like siem & EDR , we can provide training.

## Identification ( aka: detection & analysis)

This phase involves identifying if the threat is legit or not by checking alerts , and checking scope of the alerts.


### Containment

Once you identify the threat and find it legit our first step should be to stop it from spreading on to the network we can do it by disconnecting it from the network or disabling compromised account.

### Eradication 

After the threat is isolated, you must remove it entirely and return to normal operations that is what we do in eradication stage .
we can delete malware , disable breached user account and patch the vulnerabilities that allowed the attack.

## Recovery

In recovery phase we restore system from clean backups and gradually re-enable services.

### Post Incident Activity 

In post incident activities we discuss what happened how it happened and also improve our IR plan.



---



### IDS vs IPS



| Features              | Intrusion Detection system                          | Intrusion protection system                                 |
| --------------------- | --------------------------------------------------- | ----------------------------------------------------------- |
| **Primary action**    | monitors and gives alerts                           | Detects and alerts system along with blocking the intrusion |
| **response**          | manual , need human to act                          | automated , takes real-time action                          |
| **Deployment**        | IDS is deployed out of band , on a copy of traffic. | IPS is deployed inline , directly in the traffic path.      |
| **Effect on network** | Does not slows the network no effect.               | slows down the network                                      |

### Intrusion detection system 

IDS is a visibility tool that scans network for signs of breach it works by comparing the network packet against a database of known threat signatures.


**How it reacts:** When a threat is detected, it logs the event and sends an alert to your security team.

often using a SPAN or TAP port


### Intrusion Protection System

An IPS system is closely monitored and stops the attack before it can reach their target .Because it sits " inline" and every packet must pass trough it. 

**how it reacts** : It can drop malicious packet rest connections or even reconfigure a firewall to block the attackers IP automatically.


--- 
### Shared detection methods 

Both systems use the same three core method to find threats.

1. **signature-based :** it checks traffic against a  " blacklist" of known attack patterns.
   
2. **anomaly-based :** It uses machine learning to establish a baseline of normal activity and flags deviations.
   
3. **Policy-based :** It only gets activated when a specific organisation designed security rule is violated. 


---

### End-point Detection 

1. **Endpoint platform (EPP) :** end point platforms usually worked on signature based approach as they check a blacklist and compare it with current list.
   
2. **Endpoint detection response:**  in endpoint detection it works on a anomaly based approach and it keeps on monitoring an endpoint and detects if there is any malicious/suspicious activity and blocks it.

### Working of  EDR

1. **Data collection : ** an EDR program is installed in endpoint which monitores the system 24/7 what the system is doing and what files is it working on.
   
2. **Detection : **  EDR program checks behavious of this file that it finds suspicious.

3.  **Containment :**  The moment EDR detects threat it instantly isolates the system ( cuts it's internet), kills the process that caused the behaviour.

4. **Investigation & Remediation :**  After investigation EDR tells how attack got started and what was its RC(root cause ) in some cases EDR is also capable of doing a rollback for the encrypted files, rollback means if the ransomware locked the files it will bring back the file either by decrypting or backup.


>[!info] Antivirus are EPP and EDR are diffrent programs



