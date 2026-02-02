**Everything in linux is file**
**linmux works on FHS which is Filesystem Hierarchy Standard.**

**top to the tree is '    /    ' which is called root folder**

---

[No alternative text description for this image](https://media.licdn.com/dms/image/v2/D5610AQFCh_4-qkuEEw/image-shrink_800/B56ZbCpzobGsAc-/0/1747022461868?e=1769601600&v=beta&t=_kM83P-uD784rWNityOEw2H_n1SA5noNmEXeuGG5Y98)



---

### / 

Everything starts from / (root) 

## /bin

- **`/bin` (Binaries):** Contains essential executable programs required for the system to run in single-user mode and for all users (e.g., `ls`, `cp`, `bash`).

## /boot

- **`/boot` (Static Boot Files):** Stores files necessary for the boot process, including the Linux kernel (`vmlinuz`) and bootloader configuration files (e.g., GRUB).

## /dev

- **`/dev` (Device Files):** Represents hardware and virtual devices as files. For example, `/dev/sda` represents a hard drive, and `/dev/null` is a special file used to discard data.


##  /etc  (  Editable Text Configuration )

- **`/etc` (Configuration Files):** The "nerve center" of the system, housing system-wide configuration files (e.g., `/etc8/passwd` for user info or `/etc/fstab` for disk mounts).


## /home

- **`/home` (User Home Folders):** Personal directories for standard users to store their data and settings (e.g., `/home/username`).

## /root 

**`/root` (Root User Home):** The separate home directory for the superuser (system administrator). This is distinct from the system root (`/`).


## /bin

- **`/sbin` (System Binaries):** Similar to `/bin`, but contains binaries intended for system administration tasks, typically requiring root privileges (e.g., `reboot`, `iptables`).

## /usr

- **`/usr` (User Utilities) ( Unix system resources):** The largest directory, containing secondary read-only user data, including applications, libraries, and documentation.
  basically, binaries & files that are general purposely used for user operation.
## /var 

- **`/var` (Variable Data):** Stores files that are expected to change frequently over time, such as system logs (`/var/log`), caches, and spool files.


## /Temp

- **`/tmp` (Temporary Files):** A space for applications to store temporary files, which are usually cleared upon system reboot.


## /proc


- **`/proc` (Process Info):** A virtual filesystem that provides runtime information about the kernel and running processes.

## /sys

- **`/sys` (System Info):** Another virtual filesystem used to interact with and manage hardware device drivers.


## /run

- **`/run` (Runtime Data):** Stores volatile runtime data like process IDs (PIDs) since the last boot.

## /mnt 

- **`/media` & `/mnt`:** Used as mount points for external storage. `/media` is typically for automatically mounted removable media (like USB drives), while `/mnt` is for manual mounting by administrators.

## /opt

- **`/opt` (Optional):** Reserved for installing third-party software packages that do not follow the standard filesystem hierarchy.


## /srv

- **`/srv` (Service Data):** Contains site-specific data served by the system, such as files for a web server or FTP server.

## /lib

- ****/lib -**** Contains shared libraries and kernel modules required for system programs to function.

## /lost+found


****/lost+found -**** Used to store recovered fragments of corrupted files after file system checks


---
