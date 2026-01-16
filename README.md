# Cyber-security-Intern-Second-Task-ElevateLabs
## OS Security Checklist Document 

---

## 1. USER ACCOUNT MANAGEMENT 
**Action:** Created non-root user with limited privileges

**Commands executed:** sudo useradd -m -G wheel Shri
sudo passwd intern

**Result:** Non-root user 'Shri' created. Added to wheel group for sudo access but requires password. Root login disabled by default.

<img width="638" height="226" alt="Screenshot 1" src="https://github.com/user-attachments/assets/86b9e81a-3823-48c0-9a91-ee93ed4d3e49" />


---

## 2. FILE PERMISSION HARDENING
**Action:** Secured critical system fiiles and tested permissions

**Commands executed && Result:** 

<img width="745" height="597" alt="Testfile" src="https://github.com/user-attachments/assets/739d5df8-a278-406e-be8b-96bd5f427fbb" />


## 3. FIREWALL CONFIGURATION ✓
**Action:** Enabled firewalld, SSH-only access  

**Commands executed && Result:**

<img width="677" height="399" alt="FirewallConfig" src="https://github.com/user-attachments/assets/53f7a59a-3b3d-405a-b2db-e87d36a5a5bc" />


## 4. SERVICE HARDENING

**Action:** Disabled unnecessary services

**Commands executed && Result:**

<img width="870" height="900" alt="ServiceHardening1" src="https://github.com/user-attachments/assets/b5a531f2-0705-4ff6-837b-4fe8cda41fc1" />

<img width="586" height="171" alt="ServiceHardening2&#39;&#39;" src="https://github.com/user-attachments/assets/b1e992ee-8809-4bf8-b949-614815672e7a" />

---

## 5. SYSTEM UPDATES
**Command:** 'sudo pacman -Syu'

**Result:** All packages updated, security patches applied

---

## 6. PROCESS MONITORING
**Command:** 'ps aux | grep -v root'

**Result:** Reviewed non-root processes, no zombie processes

---

## 7. SSH HARDENING
**/etc/ssh/sshd_config changes:**
PermitRootLogin no
PasswordAuthentication no

**Result:** SSH key authentication only, root login prohibited

---




