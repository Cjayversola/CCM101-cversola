# Laboratory 08 - Cloud Security Engineer

**Subject:** CCM101 - Cloud Computing

**Mission:** The Cloud Security Engineer

## Mission Overview

In this laboratory activity, I learned how to secure a Linux server using the UFW (Uncomplicated Firewall). I deployed an Nginx web application and configured firewall rules to protect the server from unauthorized incoming traffic.

## Objectives

- Understand the Principle of Least Privilege.
- Identify the attack surface of a virtual machine.
- Configure UFW with a Default Deny policy.
- Allow SSH and HTTP application traffic through specific ports.
- Document firewall configurations and security practices.

## Commands Executed

```bash
docker run -d --name secure-web-app -p 8080:80 nginx

curl http://localhost:8080

sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose

sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

- Basic Linux server security.
- Deploying an Nginx Docker container.
- Using UFW to manage firewall rules.
- Managing network ports.
- Understanding server security and attack surface reduction.
- Creating technical documentation using Markdown.
