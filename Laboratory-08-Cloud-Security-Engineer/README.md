# Laboratory 08 - Cloud Security Engineer

## Mission Overview

In this laboratory activity, I worked as a Cloud Security Engineer and secured a Linux server using the UFW firewall. I configured firewall rules, allowed only the necessary services, and documented the security configuration.

## Objectives

- Understand the Principle of Least Privilege (PoLP).
- Learn what an attack surface is.
- Configure the UFW firewall on Ubuntu.
- Apply a Default Deny policy.
- Allow only SSH and Port 8080.
- Document the security process using Markdown.

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

curl http://localhost:8080
```

## Skills Learned

- Configured the UFW firewall on Ubuntu.
- Applied the Default Deny security policy.
- Allowed only required network ports.
- Verified firewall rules using UFW commands.
- Learned the importance of reducing a server's attack surface.
- Improved my GitHub Cloud Computing portfolio with security documentation.
