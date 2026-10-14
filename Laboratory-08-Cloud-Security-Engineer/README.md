# Laboratory 08: Cloud Security Engineering

## Mission Overview

This laboratory demonstrates basic host-based firewall administration on an Ubuntu server. A containerized Nginx web application is deployed as the service to protect. UFW is then configured to enforce a Default Deny policy and permit only the network traffic required for remote administration and web access.

## Objectives

- Identify common server exposure risks.
- Explain the Principle of Least Privilege and attack surface.
- Configure and activate UFW firewall policies.
- Apply specific rules for SSH and TCP port 8080.
- Verify firewall status and document security procedures.

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

This activity improved my ability to deploy a test service, configure network access restrictions, and inspect firewall rules. I also gained a better understanding of defense in depth, least privilege, and the importance of verifying security configurations after implementation.
