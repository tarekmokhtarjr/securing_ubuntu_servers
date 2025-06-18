<link href="css/bootstrap.css" rel="stylesheet"/>
<link href="css/custom.css" rel="stylesheet"/>
<h1 align="center">Securing Ubuntu Servers: A Practical Guide</h1>

<h2>Module 1: Introduction & Threat Landscape</h2>

<div class="form-check">
  <input class="form-check-input rounded-checkbox" type="checkbox" value="" id="m1_1">
  <label class="form-check-label" for="m1_1">
     Why server security matters
  </label>
</div>
<div class="form-check">
  <input class="form-check-input" type="checkbox" value="" id="m1_2">
  <label class="form-check-label" for="m1_1">
    Common attack vectors targeting Linux/Ubuntu servers
  </label>
</div>
<div class="form-check">
  <input class="form-check-input" type="checkbox" value="" id="m1_3">
  <label class="form-check-label" for="m1_1">
    Overview of Ubuntu LTS and security support lifecycle
  </label>
</div>
<div class="form-check">
  <input class="form-check-input" type="checkbox" value="" id="m1_4">
  <label class="form-check-label" for="m1_1">
    Defining the “attack surface” on a server
  </label>
</div>

<h2>Module 2: Initial Server Setup & Minimization</h2>

<li>Installing Ubuntu Server on a virtual machine</li>
<li>Updating and upgrading the system (`apt`, `unattended-upgrades`)</li>

<h2>Module 3: User & Access Control</h2>

- Creating and managing users securely

- SSH key-based authentication

- Disabling root login and password auth over SSH

- Sudo access and role separation

- Using `faillock`, `pam_tally2`, and login security measures

---

### **Module 4: Firewall and Network Hardening**

- Configuring UFW (Uncomplicated Firewall)

- Introduction to `iptables` and `nftables`

- Restricting ports and securing network interfaces

- Port knocking and VPN gateways

- Detecting and mitigating port scans (fail2ban, psad)

---

### **Module 5: File System and Process Security**

- Setting proper file and directory permissions

- Using `umask` and access control lists (ACLs)

- Mount options (`noexec`, `nosuid`, `nodev`)

- Managing running processes (`top`, `htop`, `systemctl`)

- Detecting suspicious processes

---

### **Module 6: SSH and Remote Access Security**

- Hardening `sshd_config`

- Multi-factor authentication for SSH

- SSH jump hosts and bastion best practices

- Logging and auditing remote access

---

### **Module 7: Application & Service Security**

- Hardening common services: Nginx, Apache, MySQL/PostgreSQL

- Running services with least privilege (systemd units, chroot, `no-new-privileges`)

- Using reverse proxies securely

- Updating software and mitigating CVEs

---

### **Module 8: Monitoring and Intrusion Detection**

- Setting up `auditd` and system logging

- Using `logwatch`, `logrotate`, and syslog-ng/rsyslog

- Intrusion detection with AIDE, OSSEC, or Wazuh

- System integrity checks and baseline creation

---

### **Module 9: Backup and Disaster Recovery**

- Backup tools: `rsync`, `borg`, `restic`, `duplicity`

- Encrypting backups and storing them offsite

- Automating backup schedules

- Simulating recovery and disaster scenarios

---

### **Module 10: Ongoing Security Maintenance**

- Setting up automatic security updates

- Regular auditing with `Lynis`, `chkrootkit`, `rkhunter`

- CIS benchmarks for Ubuntu

- Keeping logs, compliance checks, and documentation

---

### **Bonus Module (Optional): Advanced Hardening**

- AppArmor and SELinux (brief intro)

- Systemd sandboxing for services

- Kernel hardening (sysctl, GRUB parameters)

- Using `ufw` with rate-limiting, logging, and profiles

- Live patching with Canonical Livepatch

---

### **Final Practical Exercise**

- Hands-on: Secure a newly deployed Ubuntu server based on a checklist

- Student configures firewall, hardens SSH, installs IDS, sets up logging, etc.

- Optional security audit using automated tools
