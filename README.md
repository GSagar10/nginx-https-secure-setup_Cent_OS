# 🔐 Secure Nginx HTTPS Deployment on CentOS

**Hands-on Linux Admin Project**

I completed a **secure Nginx HTTPS setup on CentOS**, focusing on real-world security controls, troubleshooting, and validation.

This project demonstrates **defense-in-depth** at the web-server level.

---

## 📌 Project Highlights

* Secure HTTPS configuration using **SSL/TLS**
* Network-level access control (IP allow/deny)
* Application-level protection using **Basic Authentication**
* Real-world troubleshooting (port conflicts, 404 issues)
* End-to-end browser validation
* Version-controlled documentation on GitHub

---

## 🛠️ Technologies Used

* CentOS Linux
* Nginx
* OpenSSL
* httpd-tools (htpasswd)
* systemd
* Git & GitHub

---

## ⚙️ Implementation Steps (High-Level)

### 1️⃣ Install & Configure Nginx

* Installed Nginx on CentOS
* Enabled and managed service using systemd

### 2️⃣ Enable HTTPS (SSL/TLS)

* Generated self-signed SSL certificate using OpenSSL
* Configured Nginx to listen on port **443**
* Verified HTTPS from browser

### 3️⃣ Resolve Port Conflict

* Identified Apache (httpd) using port 80
* Stopped & disabled Apache
* Successfully started Nginx

### 4️⃣ Implement IP-Based Access Control

* Allowed only **192.168.44.0/24** subnet
* Denied all other traffic

### 5️⃣ Secure Application Path with Basic Auth

* Protected `/docs` path using `.htpasswd`
* Created secure credentials
* Validated authentication flow

### 6️⃣ Browser & CLI Validation

* Tested HTTPS access from browser
* Verified authentication prompts
* Validated ports and firewall rules

---

## 🔐 Security Layers Implemented

✔ SSL/TLS encryption
✔ Subnet-based network restriction
✔ Basic authentication (username/password)
✔ Service hardening & validation

---

## 🎯 Outcome

Successfully deployed a **secure, access-restricted Nginx web server** on CentOS with layered security and full browser validation.

This setup can be used for:

* Internal dashboards
* Admin panels
* Secure documentation portals

---

## 📂 GitHub Repository

🔗 **Repository:**
[https://github.com/GSagar10/nginx-https-secure-setup_Cent_OS](https://github.com/GSagar10/nginx-https-secure-setup_Cent_OS)

Includes:

* Configuration files
* Step-by-step documentation
* Commands used
* Troubleshooting notes

---

## 🧠 Key Learnings

* `nginx -t` validates syntax, not runtime port conflicts
* Self-signed certificates encrypt traffic but are not browser-trusted
* Access control does not create content (404 ≠ auth failure)
* Real Linux admin work is **debugging, not just configuration**

---

## 🚀 Next Improvements (Planned)

* HTTP → HTTPS redirection
* Let’s Encrypt SSL
* SELinux production rules
* Nginx reverse proxy setup

---

#Linux #Nginx #CentOS #DevOps #Security #HTTPS #SysAdmin #OpenSource

---

---

# 📦 GitHub Upload Steps (Clean & Correct)

Run inside your project directory:

```bash
git init
git add .
git commit -m "Secure Nginx HTTPS setup on CentOS"
git branch -M main
git remote add origin https://github.com/GSagar10/nginx-https-secure-setup_Cent_OS.git
git push -u origin main
```





