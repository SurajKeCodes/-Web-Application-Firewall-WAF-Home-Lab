
# 🛡️ Web Application Firewall (WAF) Home Lab

**WAF Home Lab** is a hands-on cybersecurity project that simulates real-world web attacks and demonstrates how a Web Application Firewall (WAF) protects applications against malicious traffic.
<h2 align="center">📸 Project Screenshots</h2>

<p align="center">
  <table align="center" cellspacing="10">
    <tr>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/80c5bedd-4656-4d0c-8a95-9d10ed7b8854" width="100%" />
      </td>
      <td align="center">
        <img src="https://github.com/user-attachments/assets/fd2a36a5-ca7d-4e60-82d3-80c37eb6a409" width="100%" />
      </td>
    </tr>
  </table>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/271e8587-6141-46c7-ba4a-d2d7b1d1640f" width="80%" />
</p>


---

## 📌 Overview

This lab environment consists of:

- **Kali Linux** (Attacker Machine)  
- **Ubuntu Server** (Target System)  
- **DVWA** (Damn Vulnerable Web Application)  
- **SafeLine WAF** (Security Layer)  

It showcases an end-to-end **attack → detection → defense workflow**.

---

## 🏗️ Architecture

```

[ Kali Linux (Attacker) ]
↓
[ SafeLine WAF (Reverse Proxy + Protection) ]
↓
[ Ubuntu Server (DVWA running on port 8080) ]

````

---

## ✨ Key Features

- Simulated real-world attacks like **SQL Injection**  
- Deployed and configured **SafeLine WAF as reverse proxy**  
- Protected backend DVWA application running on custom port (8080)  
- Monitored and analyzed **WAF logs and blocked requests**  
- Implemented:
  - IP blocking rules  
  - HTTP flood (DoS) protection  
  - Authentication layer  

---

## ⚙️ Tech Stack

- Kali Linux  
- Ubuntu Server  
- DVWA (Damn Vulnerable Web Application)  
- SafeLine WAF  
- VirtualBox  
- LAMP Stack (Linux, Apache, MySQL, PHP)  
- Networking (Bridged Adapter)  

---

## 🎯 Objectives

- Simulate real-world cyber attack scenarios  
- Perform SQL Injection attacks from Kali Linux  
- Deploy and configure a Web Application Firewall  
- Analyze WAF behavior under malicious traffic  

---

## 🔧 Setup Overview

### 1. Virtual Environment
- Created Kali Linux and Ubuntu Server using VirtualBox  
- Configured **bridged networking for same network communication**  

### 2. Server Setup
- Installed LAMP stack (Apache, MySQL, PHP)  
- Deployed DVWA on Ubuntu  
- Configured DVWA to run on **port 8080**  

### 3. WAF Deployment
- Installed SafeLine WAF using automated script  
- Configured **reverse proxy → backend (DVWA)**  
- Enabled HTTPS using self-signed SSL certificate  

### 4. DNS Configuration
- Configured `/etc/hosts` for local domain resolution (`dvwa.local`)  

---

## ⚔️ Attack Demonstration

Example SQL Injection payload:

```sql
admin' OR '1'='1
````

* Performed login bypass attack on DVWA
* Generated malicious HTTP requests from Kali Linux

---

## 🛡️ Defense Results

* SafeLine WAF successfully:

  * Detected SQL Injection attempts
  * Blocked malicious requests
  * Logged attack activity

* Verified real-time traffic filtering and protection

---

## 📊 Results

* Built a complete **attack-defense cybersecurity lab**
* Demonstrated practical WAF protection mechanism
* Gained hands-on experience with real-world tools

---

## 🧠 Key Learnings

* Working of Web Application Firewalls (WAF)
* Reverse proxy security architecture
* Attack simulation and mitigation techniques
* Traffic monitoring and filtering

---

## 🚀 Future Improvements

* Add XSS and File Inclusion attacks
* Integrate SIEM tools for log analysis
* Automate attack testing
* Deploy OWASP Juice Shop

---

## 🤝 Connect With Me

<p align="left">
  <a href="https://linkedin.com/in/surajborkute" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:surajborkute@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://wa.me/9518772281" target="_blank">
    <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" />
  </a>
  <a href="https://suraj-borkute-portfolio.vercel.app/" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" />
  </a>
</p>

---

## 👨‍💻 Author

**Suraj Borkute**
Cybersecurity Enthusiast | Networking | GATE Aspirant 🚀

---

## ⚠️ Disclaimer

This project is for educational purposes only.
All attacks were performed in a controlled lab environment.

---

## 📄 License

This project is licensed under the MIT License.

---
