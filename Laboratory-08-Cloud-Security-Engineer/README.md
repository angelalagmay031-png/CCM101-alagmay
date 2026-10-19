# Laboratory 08 - Cloud Security Engineer

## Mission Overview

The mission of this laboratory was to secure a web server using UFW (Uncomplicated Firewall). I configured firewall rules to control incoming and outgoing traffic and allowed the necessary ports for SSH administration and web application access.

## Objectives

- Understand the importance of firewall configuration in cloud security.
- Allow SSH connections for remote server administration.
- Apply the Default Deny policy for incoming traffic.
- Allow outgoing traffic from the server.
- Open TCP port 8080 for the Nginx web application.
- Verify firewall rules and test the web application using curl.

## Commands Executed

```bash
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

In this laboratory, I learned how to configure and activate a firewall using UFW in Ubuntu. I also learned how to apply the Default Deny policy, allow specific ports, and check firewall rules. Testing the Nginx web application with curl helped me understand the importance of verifying services after configuring security settings.
