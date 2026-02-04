# Process

#### **Every command executed or application launched creates one or more processes**

#### A **process** is an instance of a running program, while a **service** (often called a **daemon**) is a type of background process designed to provide specific system functionalities. 

#### Processes are managed by the kernel, while services are typically managed by an init system like `systemd` on modern distributions.

---
#### " Hinglish "

## Process running program ka aak hissa hota hai 

## Service / daemon aak background process hota hai jo kee spesific task perform Karta h


## **Process States** : 

1. **Running (R)**

2. **Sleeping (S)**

3. **Uninterruptible Sleep (D)**

4. **Stopped**

In linux ps tool  is used to to see process in linux.

```

ps 
ps aux 
ps -ef
```

 ---
### PS Tool 

[](https://www.testingdocs.com/wp-content/uploads/ps-Linux-command-1536x710.png)







- ****UID****: User ID that this process belongs to (the person running it)
- ****PID****: Process ID
- ****PPID****: Parent process ID (the ID of the process that started it)
- ****C****: CPU utilization of process
- ****STIME****: Process start time
- ****TTY****: Terminal type associated with the process
- ****TIME****: CPU time is taken by the process
- ****CMD****: The command that started this process


--- 

### Types of Processes

There are three types of Processes

1. Parent and Child process
2. Zombie and Orphan process
3. Daemon process


## Parent and Child process

A normal process and its sub process , the sub process is child process and the process which is doing it is parent.

## Zombie and Orphan process

When a child process finishes work and sends signal to parent to terminate it , but the parent process is already  terminated before terminating child process in this case the child process is orphan.

## Daemon process

Background process that runs with root permission is called a daemon process.


---


### systemd
