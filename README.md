# 🚀 Deploying an NGINX Web Server on AWS EC2 with a Custom Domain using Cloudflare 🌐

For this Networking module, I deployed my own NGINX web server on an AWS EC2 instance and connected it to a custom domain purchased through Cloudflare.

In this write-up, I’ll walk you through every stage of the process: from buying the domain to setting up DNS records, configuring the server, and customising the landing page. 

---

## 🌍 Live Demo
**Visit my project:** http://nginxjawwad.org/  
*(This demo will only be live temporarily for the Networking module)*

![Project Screenshot](images/final-photo-nginx.png)

---

## Stage 1 – Purchased a Domain

I bought a domain using **Cloudflare** to use for my NGINX web server project.

**Steps:**
1. Logged into Cloudflare.
2. Purchased a new domain name.
3. Prepared it for linking to my server later.

![Stage 1: Domain Purchase in Cloudflare](images/stage1-domain.png)

## Stage 2 – Launched EC2 Instance and Installed NGINX

I set up an AWS EC2 instance and installed NGINX to serve web content.

**Steps:**
1. Opened AWS EC2 dashboard.
2. Launched a new instance using Amazon Linux 2.
3. Selected t2.micro (free tier) instance type.
4.  Configured security group rules to allow inbound HTTP (port 80) from 0.0.0.0/0.
5. Connected using AWS EC2 Instance Connect in the browser.
6. Installed NGINX by running these commands:

   ```bash
   sudo yum -y install nginx
   sudo systemctl start nginx
   sudo systemctl enable nginx

7. I then confirmed if nginx was running :
 
    ```bash
    systemctl status nginx
