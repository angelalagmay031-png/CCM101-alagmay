
# Firewall Configuration

## 1. Allow SSH Access

Command used:

```bash
sudo ufw allow ssh
```

This command allows SSH connections on port 22 so administrators can remotely manage the server.

## 2. Set the Default Deny Policy

Commands used:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command blocks incoming connections unless they are explicitly allowed, while the second command allows outgoing connections from the server.

## 3. Allow Port 8080

Command used:

```bash
sudo ufw allow 8080/tcp
```

This command allows incoming TCP traffic on port 8080 so users can access the Nginx web application.

## 4. Activate and Verify the Firewall

Commands used:

```bash
sudo ufw enable
sudo ufw status verbose
sudo ufw status numbered
```

These commands activate the firewall, check its status and default policies, and display the configured firewall rules.

## 5. Importance of Allowing SSH First

If I run `sudo ufw enable` before `sudo ufw allow ssh`, incoming SSH connections may be blocked, which could lock me out of the server if I am managing it remotely.
