
### log

A log file is a computer-generated record of events, activities, and operations within a system, application, or server.

### Types of logs

#### 1. System logs 
#### 2. Authentication logs
#### 3. application logs

#### - `/var/log/kern.log`: Kernel messages and errors, useful for more advanced investigations
#### - `/var/log/syslog (or /var/log/messages)`: A consolidated stream of various Linux events
#### - `/var/log/dpkg.log (or /var/log/apt)`: Package manager logs on Debian-based systems
#### - `/var/log/dnf.log (or /var/log/yum.log)`: Package manager logs on RHEL-based systems


---

### System logs

system log provides information about operating system like startup/shutdown messages , errors , warning , and various message from daemon and the kernel.

#### Example 


```

Jan 23 14:12:45 server1 sshd[2345]: Failed password for root from 45.67.89.10 port 54321 ssh2


```


- **Time** → `Jan 23 14:12:45`
    
- **Machine name** → `server1`
    
- **Program** → `sshd`
    
- **PID** → `[2345]`
    
- **Actual event** → `Failed password for root from 45.67.89.10`

> We can use tools like less grep tail to find what we need in log file instad of going trough whole file.

### Use `grep -E '(passwd | Passwd)' ` "-E " flag to use regex expressions

> .bash_history : file tell history of commands used since system booted for current instance.

---

###  Authentication log 

##### Logs related to **authentication and authorization**.

[Referance image](https://tryhackme-images.s3.amazonaws.com/user-uploads/678ecc92c80aa206339f0f23/room-content/678ecc92c80aa206339f0f23-1755091674006.svg)


```
Jan 23 14:12:45 server1 sshd[2345]: Failed password for root from 45.67.89.10 port 54321 ssh2

```

- **Timestamp** → Jan 23 14:12:45
    
- **Host** → server1
    
- **Process** → sshd[2345]
    
- **Message** → Failed password for root from IP