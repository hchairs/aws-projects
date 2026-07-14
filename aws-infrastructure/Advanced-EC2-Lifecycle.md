# My Hands-On Experience with AWS EC2: Managing a Server Lifecycle
**By Harold Chairs**  
**Date:** July 14, 2026  

---

## 🚀 What I Did
I wanted to get my hands dirty with real-world cloud infrastructure, so I spun up a web server on Amazon Web Services (AWS) and took it through its entire lifecycle. Instead of just launching it and leaving it, I configured security firewall rules, tested safety features, scaled the performance up, and properly shut it down.

## 🛠️ The Skills I Practiced
* **Cloud Security:** Fixing firewalls so real people can access a web server.
* **Server Safety:** Setting up guardrails so critical servers don't get deleted by accident.
* **Scaling:** Resizing a virtual machine on the fly when you need more power.
* **Monitoring:** Reading cloud dashboards to make sure everything is running healthy.

---

## 📝 Walkthrough of My Project

### 1. Launching and Protecting the Server
I started by launching a brand new Amazon EC2 instance to act as my web server. Right out of the gate, I enabled **Termination Protection**. This is a great safety feature that prevents you (or anyone else) from accidentally deleting the server with a wrong click.

### 2. Opening Up Web Traffic
At first, the server was locked down. I went into the **Security Group** settings and added a rule to allow **HTTP access on Port 80**. This opened the front door so the public internet could actually load my web page. I also checked the console dashboard to ensure the system passed its health checks.

### 3. Scaling the Server Up
To see how easy it is to handle a traffic spike, I decided to vertically scale the server. I safely stopped the instance, changed its size to a larger instance type to give it more computing power, and turned it back on. 

### 4. Testing the Safeguards & Cleaning Up
Finally, I tried to delete the running server to see if my safety settings worked. AWS blocked me immediately, proving that **Termination Protection** does its job. Once I verified that worked, I manually turned off the protection and terminated the instance so I wouldn't run up an unexpected bill.



