# 🚀 Deploying an NGINX Web Server on AWS EC2 with a Custom Domain using Cloudflare 🌐

For this Networking module, I deployed my own NGINX web server on an AWS EC2 instance and connected it to a custom domain purchased through Cloudflare.

In this write-up, I’ll walk you through every stage of the process: from buying the domain to setting up DNS records, configuring the server, and customising the landing page. 

---

## 🌍 Live Demo
**Visit my project:** http://nginxjawwad.org/  
*(This demo will only be live temporarily for the Networking module)*

![Project Screenshot](images/final-photo-nginx.png)

---

## Stage 1 – Purchased a Domain and Linked it to My AWS EC2 Instance

I bought a domain using Cloudflare and linked it to my EC2 instance so the site can be accessed by domain name.

**Steps:**
1. Bought domain on Cloudflare.
2. Added an **A record** pointing to my EC2 public IPv4.
3. Allowed inbound **HTTP (port 80)** in EC2 security group.
4. Waited for DNS to update and tested in browser.

![Stage 1: Domain Overview in Cloudflare](images/stage1-domain.png)
